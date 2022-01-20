---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2921ce29d5c6e12399eac9b7e3f4519d7dfc779f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123633"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignment -EducationClassId $educationClassId -ExpandProperty "resources" 

```