---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d7817bfcdc78de0b7f6aa98018cc16c2713508c
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509620"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemInsights = await graphClient.Organization["{organizationId}"].Settings.ItemInsights
    .Request()
    .GetAsync();

```