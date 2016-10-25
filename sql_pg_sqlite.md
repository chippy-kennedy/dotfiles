#PG
##Linux
####Change User Password from Linux
`sudo -u <pg_username> psql`

`psql> ALTER USER <pg_username> PASSWORD '<new_password>'`



##Mac OSX
####Start/Stop psql server via Brew
>http://stackoverflow.com/questions/7975556/how-to-start-postgresql-server-on-mac-os-x

#MYSQL2
##Linux
####Monkey Patch Rails 3 with Current Mysql2
```
#config/initalizers/abstract_mysql2_adapter.rb
class ActiveRecord::ConnectionAdapters::ColumnDefinition
  def sql_type
    type.to_sym == :primary_key ? 'int(11) auto_increment PRIMARY KEY' : base.type_to_sql(type.to_sym, limit, precision, scale) rescue type
  end 
end
```
