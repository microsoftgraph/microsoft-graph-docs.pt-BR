---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41f6ff60e40180d8d54d4ff8f15a3d591744f6d0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135795"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupThreadPostAttachment -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId

```