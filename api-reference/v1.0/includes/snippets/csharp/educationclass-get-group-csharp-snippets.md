---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 153b0280c04a9d48467d62ead93e6dccbc372dea
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422227"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Education.Classes["{class-id}"].Group
    .Request()
    .GetAsync();

```