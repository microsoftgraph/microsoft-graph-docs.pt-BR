---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17d63a8122c1823785c8c1767632e10453ffde3792cdeb103b1f18b2ad4e30c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @string = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Operations["{ediscovery.caseOperation-id}"]
    .GetDownloadUrl()
    .Request()
    .GetAsync();

```