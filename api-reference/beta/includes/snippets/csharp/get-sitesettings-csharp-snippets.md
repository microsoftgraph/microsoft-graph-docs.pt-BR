---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2f1013edde8f2e22b0c4d2ca9a4f4ed7a2df9ab
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211177"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites["{site-id}"]
    .Request()
    .Select("Settings")
    .GetAsync();

var settings = sites.Settings;

```