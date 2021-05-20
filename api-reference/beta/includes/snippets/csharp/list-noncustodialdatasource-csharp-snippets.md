---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd71698b9aac5881ec331f96935ea3f58286b3b9
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52563837"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialDataSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources
    .Request()
    .GetAsync();

```