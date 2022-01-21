---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2ba2e41555b60d01438b4b61f53f0d3ddc0b6729
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112857"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupThreadPostExtension -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -ExtensionId $extensionId

```