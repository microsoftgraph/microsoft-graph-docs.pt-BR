---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28aeb51e9b3284708e9d37c59499e8bcd2147d76a5636c5d828f08d52d84424a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewers = await graphClient.AccessReviews["{accessReview-id}"].Reviewers
    .Request()
    .GetAsync();

```