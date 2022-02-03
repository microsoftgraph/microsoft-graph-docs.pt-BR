---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be08186d0e8143ffd388fe24b16f6f0f71a9f95a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349944"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessage -UserId $userId -Property "subject,body,bodyPreview,uniqueBody" 

```