---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37429800faeb3c7c6dc4cc36c74ea9b0b89726cc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageAccountDetail = await graphClient.Reports.GetOneDriveUsageAccountDetail('D7')
    .Request()
    .GetAsync();

```