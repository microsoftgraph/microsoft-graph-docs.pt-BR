---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aadaf523d3a4f1fa8c67dd6ba1587a126cb5eb53
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Columns
    .Request()
    .GetAsync();

```