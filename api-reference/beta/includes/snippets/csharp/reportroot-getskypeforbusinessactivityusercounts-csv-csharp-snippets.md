---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a5ef9e15533afe61fe271845f2c866f27a91aa0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499255"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityUserCounts = await graphClient.Reports.GetSkypeForBusinessActivityUserCounts('D7')
    .Request()
    .GetAsync();

```