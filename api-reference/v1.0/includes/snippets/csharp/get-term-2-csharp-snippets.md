---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c43e5ed6c769c6da59b084a4c17d304ead0a38a2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094576"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"].Children
    .Request()
    .GetAsync();

```