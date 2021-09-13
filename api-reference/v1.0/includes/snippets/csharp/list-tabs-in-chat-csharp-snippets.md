---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0901e50f36d292c939a064f2db26fa3ef533a162608296b3c14d30549a38166d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900142"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Chats["{chat-id}"].Tabs
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```