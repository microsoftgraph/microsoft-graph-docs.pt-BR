---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be650d47890c14e974c31c6164137a3a2fa7b7e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365GroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```