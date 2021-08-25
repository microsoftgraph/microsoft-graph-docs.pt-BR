---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc07acb54a02d6614ef0371f60cbf3764138b81acb0277c3a0af019d2a9b022c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"].Threads
    .Request()
    .GetAsync();

```