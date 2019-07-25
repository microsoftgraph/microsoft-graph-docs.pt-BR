---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 598cffaa494bf6c67c9e17ca9d691fed6c7c170b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873257"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityStorage = await graphClient.Reports
    .GetOffice365GroupsActivityStorage('D7')
    .Request()
    .GetAsync();

```