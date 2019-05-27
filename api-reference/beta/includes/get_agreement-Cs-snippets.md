---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d53196e7e602f2f90183c5e95d8206bacf57c33
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = await graphClient.Agreements["'id'"]
    .Request()
    .Expand("files")
    .GetAsync();

```