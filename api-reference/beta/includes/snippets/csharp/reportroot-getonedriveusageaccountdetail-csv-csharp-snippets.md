---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78087b522b70f43c0e84e4dc4a894d94eb4852ea
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageAccountDetail = await graphClient.Reports
    .GetOneDriveUsageAccountDetail('D7')
    .Request()
    .GetAsync();

```