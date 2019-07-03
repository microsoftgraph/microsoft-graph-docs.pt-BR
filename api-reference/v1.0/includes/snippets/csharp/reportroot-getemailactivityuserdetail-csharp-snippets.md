---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 881e643f93eddc41593d8db5d8c14cc3a8654b1d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailActivityUserDetail('D7')
    .Request()
    .GetAsync();

```