---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd922ccd946705b49c1a02c24511801d35e3de84
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = await graphClient.Devices["{id}"]
    .Request()
    .GetAsync();

```