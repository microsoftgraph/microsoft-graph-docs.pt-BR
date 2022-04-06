---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 669e7487770d3be86795532c45aa2066d4514a9f
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759182"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMessage -ChatId $chatId -Top 2 -Sort "createdDateTime desc" 

```