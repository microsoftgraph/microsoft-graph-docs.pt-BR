---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8358f39f16e0ca0658ef7a3a2aa21c9fc2b2811
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAddress = await graphClient.Me.Profile.Addresses["{id}"]
    .Request()
    .GetAsync();

```