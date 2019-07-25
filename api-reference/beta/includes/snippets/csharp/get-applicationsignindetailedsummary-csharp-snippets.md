---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b0d05b4c0a9df13a0ae16d56704747a4d30a07d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationSignInDetailedSummary = await graphClient.Reports.ApplicationSignInDetailedSummary["'id'"]
    .Request()
    .GetAsync();

```