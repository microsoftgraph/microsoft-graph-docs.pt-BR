---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6800d02b97219891cf6814493795a968cd5bf1b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResources = await graphClient.OnPremisesPublishingProfiles["{publishingType}"].PublishedResources
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```