---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 981c39e21964ef8cd9a3629c0ed32a9edaf639bba6ee89e1fd580d40ad205cf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330039"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

await graphClient.Me.Messages["{message-id}"]
    .ReplyAll(null,comment)
    .Request()
    .PostAsync();

```