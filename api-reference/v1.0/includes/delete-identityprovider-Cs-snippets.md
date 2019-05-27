---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2510def09068f4edb0cf9977874474c3af11b1a4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459825"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityProviders["Amazon-OAuth"]
    .Request()
    .DeleteAsync();

```