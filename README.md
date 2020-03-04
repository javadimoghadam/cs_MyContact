## My Contacts is  Software for viewing contacts, categories and ... in Windows 

Please [forks](github.com/javadimoghadam/cs_MyContacts) me On **Git Hub**

# Installation

Use the [Visual Studio](https://visualstudio.com) "Preferably Version 2017" For Open mycontacts.sln \
Use the [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) for create **Database & Table**

# Usage

> Use Below code for **Start**

```bash
Step 1 => git clone https://github.com/javadimoghadam/cs_MyContacts.git
Step 2 => cd cs_MyContacts/
Step 3 => start Mycontacts.sln
```

> **then** For Create Database use below Code

```sql
CREATE DATABASE Contact_DB
USE [Contact_DB]
GO
SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
SET ANSI_PADDING ON
GO
CREATE TABLE [dbo].[MyContacts](
	[ContactID] [int] IDENTITY(1,1) NOT NULL,
		[Name] [nvarchar](250) NOT NULL,
		[Family] [nvarchar](250) NOT NULL,
		[Mobile] [varchar](50) NOT NULL,
		[Email] [nvarchar](250) NOT NULL,
		[Age] [int] NOT NULL,
		[Address] [nvarchar](max) NULL,
		CONSTRAINT [PK_MyContacts] PRIMARY KEY CLUSTERED (
		[ContactID] ASC
		)WITH (PAD_INDEX  = OFF, STATISTICS_NORECOMPUTE  = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS  = ON, ALLOW_PAGE_LOCKS  = ON) ON [PRIMARY]
		) ON [PRIMARY]
		GO
		SET ANSI_PADDING OFF
		GO
```
## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.

**Ali Javadi 2020**

