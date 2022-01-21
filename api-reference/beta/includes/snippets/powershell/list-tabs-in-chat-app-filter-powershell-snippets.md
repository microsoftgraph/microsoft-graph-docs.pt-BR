---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5614f472f151aa51f4ddb4737fdee94ab40553a2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103804"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatTab -ChatId $chatId -ExpandProperty "teamsApp" -Filter "teamsApp/id eq 'com.microsoft.teamspace.tab.web'" 

```