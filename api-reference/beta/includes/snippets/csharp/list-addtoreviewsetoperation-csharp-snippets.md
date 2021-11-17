---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b79142a700671a3ce09c44470b9a0cddca801b81ecb59730a14b8cfaeb73ed43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addToReviewSetOperation = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].AddToReviewSetOperation
    .Request()
    .GetAsync();

```