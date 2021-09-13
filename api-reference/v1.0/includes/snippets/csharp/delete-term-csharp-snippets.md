---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 957e8a0845d7a6454a3d0bbc9c3b7f401d154ef8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
    .Request()
    .DeleteAsync();

```