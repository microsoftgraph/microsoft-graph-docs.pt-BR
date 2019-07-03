---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 351f13b9ecfb7412fbbbb6473edb1ac324b8142c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465371"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ActivationsUserDetail()
    .Request()
    .GetAsync();

```