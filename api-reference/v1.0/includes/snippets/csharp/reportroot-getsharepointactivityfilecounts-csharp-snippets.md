---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77b02c2d420d6d0b7c4a2aec353dfd7fcd9c8ec2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointActivityFileCounts('D7')
    .Request()
    .GetAsync();

```