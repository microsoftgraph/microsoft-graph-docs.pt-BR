---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 715948128a3f9a6b0ac16785a459219529ff8955
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507560"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.InferenceClassification.Overrides["98f5bdef-576a-404d-a2ea-07a3cf34af4r"]
    .Request()
    .DeleteAsync();

```