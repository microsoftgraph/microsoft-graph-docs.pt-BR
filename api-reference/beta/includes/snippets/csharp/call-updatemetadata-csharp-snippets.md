---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9d6b4894a37d4c48e837692e989404ad34ef57f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605003"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var metadata = "metadata-value";

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .UpdateMetadata(metadata,clientContext)
    .Request()
    .PostAsync();

```