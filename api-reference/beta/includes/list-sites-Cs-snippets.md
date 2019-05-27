---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b26d2568c57f8bbf0086ce27742ae6a521d86d78
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites
    .Request()
    .Filter("siteCollection/root ne null")
    .GetAsync();

```