---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9d6b4894a37d4c48e837692e989404ad34ef57f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456148"
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