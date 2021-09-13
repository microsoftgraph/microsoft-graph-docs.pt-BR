---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9060a0c8baa025c7c77637d2be6996efd10ff2cd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var relations = await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"].Relations
    .Request()
    .GetAsync();

```