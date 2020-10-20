---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57053e983723b4e3e2bd1eff607dc0dbde76f0c9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611370"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .Request()
    .DeleteAsync();

```