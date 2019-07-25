---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46f99ab44f7f0a58d58f1055002d37c53e26aee2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872526"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageStorage = await graphClient.Reports
    .GetSharePointSiteUsageStorage('D7')
    .Request()
    .GetAsync();

```