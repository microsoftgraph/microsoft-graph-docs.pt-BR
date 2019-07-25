---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b666907f3d7993c3be38c3413fad67ae51dde8e3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterOperators = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema
    .FilterOperators()
    .Request()
    .GetAsync();

```