---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76a687d6c802325a064108e81c253f738c44e6d2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = await graphClient.Settings
    .Request()
    .GetAsync();

```