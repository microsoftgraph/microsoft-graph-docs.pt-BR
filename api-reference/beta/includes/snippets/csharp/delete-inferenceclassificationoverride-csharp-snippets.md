---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 715948128a3f9a6b0ac16785a459219529ff8955
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711571"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.InferenceClassification.Overrides["98f5bdef-576a-404d-a2ea-07a3cf34af4r"]
    .Request()
    .DeleteAsync();

```