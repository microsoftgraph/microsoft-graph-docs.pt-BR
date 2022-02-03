---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: defafe13ae22fa1a2038206afab13254fb022026
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350521"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileNote -UserId $userId -PersonAnnotationId $personAnnotationId

```