---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4fc0ec909640dd31ef95f90c63430aae11d8a22b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100538"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMessage -ChatId $chatId -Top 2 -Sort "createdDateTime" 

```