---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9dede54f1539f4c234016501870f38dfc615bc60eb116f86d2710b38b1d30c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var boolean = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .IsPublished()
    .Request()
    .GetAsync();

```