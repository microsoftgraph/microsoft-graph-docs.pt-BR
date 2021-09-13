---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 808fb1fc890d1e72bc54d396887b1dc211c36ec3644f91f10573a5386ecec875
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .CreateReply(null,null)
    .Request()
    .PostAsync();

```