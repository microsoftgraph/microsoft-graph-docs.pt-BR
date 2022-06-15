---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02042a98592344e3a39d5635490b833aaad7bace
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092777"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].NoncustodialDataSources["{security.ediscoveryNoncustodialDataSource-id}"]
    .UpdateIndex()
    .Request()
    .PostAsync();

```