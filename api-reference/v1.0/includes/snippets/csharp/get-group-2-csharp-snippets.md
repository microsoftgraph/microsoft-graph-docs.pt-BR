---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdc72690545cd73eaac490c378f58205971d38c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025746"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Sites["{site-id}"].TermStore.Groups
    .Request()
    .GetAsync();

```