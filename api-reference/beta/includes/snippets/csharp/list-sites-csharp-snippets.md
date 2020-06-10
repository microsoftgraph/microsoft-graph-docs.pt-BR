---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd3a8a179254b1d71d50f6e15ea627e9cfe3b881
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites
    .Request()
    .Filter("siteCollection/root ne null")
    .Select("siteCollection,webUrl")
    .GetAsync();

```