---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec335275350f6a9241699c10e56d3abe86b4c5dbff758c264feb12d6f76641c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159712"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{call-id}"]
    .CancelMediaProcessing(clientContext)
    .Request()
    .PostAsync();

```