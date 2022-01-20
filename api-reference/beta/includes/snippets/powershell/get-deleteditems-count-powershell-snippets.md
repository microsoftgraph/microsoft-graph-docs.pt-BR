---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71b1fa25b70c9974f2814e43c223d53118d72b44
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090676"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryDeletedItem -DirectoryObjectId $directoryObjectId -CountVariable CountVar -Sort "deletedDateTime asc" -Property "id,displayName,deletedDateTime" 

```