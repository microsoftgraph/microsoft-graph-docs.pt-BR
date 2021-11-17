---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf166f59f04fdac3fd073cdf31566e90f1a3946f1006515a0f8efa71ff50863f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898023"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialDataSource = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources["{ediscovery.noncustodialDataSource-id}"]
    .Request()
    .GetAsync();

```