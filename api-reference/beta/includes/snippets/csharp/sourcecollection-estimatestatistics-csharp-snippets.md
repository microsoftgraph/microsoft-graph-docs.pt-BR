---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f85b42893c564bff6b7cf99d86197a27f6be8da7eb4841f723cdbb93273bbdee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272351"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"]
    .EstimateStatistics()
    .Request()
    .PostAsync();

```