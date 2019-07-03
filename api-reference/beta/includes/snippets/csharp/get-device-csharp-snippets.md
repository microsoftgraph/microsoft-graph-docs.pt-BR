---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd922ccd946705b49c1a02c24511801d35e3de84
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518331"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = await graphClient.Devices["{id}"]
    .Request()
    .GetAsync();

```