# Konwencja nazw zasobów w Azure dla firmy Global Cloud Corporation

## Słownik

### \<companyprefix>

* Global Cloud Corporation = gcc

### \<branch>

* Hiszpania = es
* Wielka Brytania = uk
* Polska = pl
  
### \<department>

* HumanResource = hr
* CyberSecurity = cs
* Infromation Technology = it
* Research & Development = rd
  
### \<team>

* DevTeamOne = dt1
* OperationTemOne = ot1

### \<solution>

* Customer relationship management = crm
* Electronic Health Record = ehr

### \<vm_os>

* Windows = w
* Linux = l
  
### \<vm_service>

* DataBase = dbs
* Remote Desktop Services = rds
* Web Application =  web
* .Net Service Bus = nsb

### \<env>

* Produkcja = prd
* PreProd = pre
* Development = dev

### \<object_number>

* <001..999>

## Przykłady

### Resource group

\<companyprefix>\<branch>-\<env>\(\<department>\<team>\<solution>\)-rg-\<object_number>

* gccpl-prd-rg-001
* gcces-pre-hr-rg-001
* gcces-pre-hr-rg-001
* gccuk-pre-rd-dt1-rg-001
* gccuk-dev-rd-dt1-ehr-rg-001

### VNET

\<companyprefix>\<branch>-\<env>\(\<department>\<team>\<solution>\)-vnet-<object_number>

* gccuk-pre-rd-dt1-vnet-001

### Virtual machine (\<vm_name>)

\<companyprefix>\<branch>\<env>\(\<department>\<team>\<solution>\)vm\<vm_os>\<vm_service>\<object_number>

* gccukdevrddt1vmwnsb001
* gccukdevrddt1ehrvmwdbs001

### Disk

#### OS Disk

* <vm_name>_OsDisk
  
#### Data Disk

* <vm_name>\_DataDisk\_\<object_number>

### Storage Account

\<companyprefix>\<branch>\<env>\(\<department>\<team>\<solution>\)sa\<object_number>

* gccukdevrddt1sa001
