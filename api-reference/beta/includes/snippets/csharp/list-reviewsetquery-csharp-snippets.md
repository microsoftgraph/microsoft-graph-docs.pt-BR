---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e53e86222da352d4ca4858b1fd0372c4608b5fa9b4daa9209d85412a7d9e2750
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queries = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"].Queries
    .Request()
    .GetAsync();

```