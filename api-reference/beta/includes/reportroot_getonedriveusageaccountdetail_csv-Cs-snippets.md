---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37429800faeb3c7c6dc4cc36c74ea9b0b89726cc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441000"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageAccountDetail = await graphClient.Reports.GetOneDriveUsageAccountDetail('D7')
    .Request()
    .GetAsync();

```