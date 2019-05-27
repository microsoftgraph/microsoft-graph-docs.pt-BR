---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f06acd154b19fbc5676645059d41fe9e6e612be3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMembers = await graphClient.Groups["{id}"].TransitiveMembers
    .Request()
    .GetAsync();

```