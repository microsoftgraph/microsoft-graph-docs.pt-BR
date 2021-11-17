---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8022620c765eff3ecaf423d7fee270a7eb0c56e3a798e8cada01f7d1d7e2a0fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = new AccessReview
{
    DisplayName = "TestReview new name"
};

await graphClient.AccessReviews["{accessReview-id}"]
    .Request()
    .UpdateAsync(accessReview);

```