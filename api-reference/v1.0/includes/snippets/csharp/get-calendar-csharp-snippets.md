---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4692306cd41c8a719334c5e844bf47b00b98cc4c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465775"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = await graphClient.Me.Calendar
    .Request()
    .GetAsync();

```