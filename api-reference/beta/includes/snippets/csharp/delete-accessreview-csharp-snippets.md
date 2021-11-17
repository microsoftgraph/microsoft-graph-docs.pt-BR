---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08fbb53dee3c321a1521c2af7d99662566504183143fcd20e88d0990bb472b16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .Request()
    .DeleteAsync();

```