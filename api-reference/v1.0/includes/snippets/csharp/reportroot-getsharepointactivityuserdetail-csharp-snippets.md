---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 795a047824a0f5ca7b593a65ebec5d8bdd895861
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointActivityUserDetail('D7')
    .Request()
    .GetAsync();

```