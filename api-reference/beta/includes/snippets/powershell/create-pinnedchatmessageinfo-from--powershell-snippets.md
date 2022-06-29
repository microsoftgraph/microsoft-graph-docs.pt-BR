---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f3cf9a24d425c4ea6266e71c16558ef0b80ae6b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441242"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Message@odata.bind" = "https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616964509832"
}

New-MgChatPinnedMessage -ChatId $chatId -BodyParameter $params

```