---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d43494b96335439946c46ac7877a7f8d21ceb75d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105713"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfile -UserId $userId -ExpandProperty "names(`$select=first,last),skills(`$select=displayName)" 

```