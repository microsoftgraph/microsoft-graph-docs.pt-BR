---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15c62d0c9d84dcee968247047b40dc92e3f4e0e6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getRecentNotebooks = await graphClient.Me.Onenote.Notebooks
    .GetRecentNotebooks(true)
    .Request()
    .GetAsync();

```