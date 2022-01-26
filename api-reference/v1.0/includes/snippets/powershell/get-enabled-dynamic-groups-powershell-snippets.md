---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0b5babe3530016980210b73d8dcb0279c8e5472
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62225601"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroup -Filter "mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'" -CountVariable CountVar -Property "id,membershipRule,membershipRuleProcessingState" -ConsistencyLevel eventual 


```