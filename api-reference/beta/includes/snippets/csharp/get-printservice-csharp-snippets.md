---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e9a7a2066d32dfd4066c0ad8deb6999f777773a
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42947539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printService = await graphClient.Print.Services["{id}"]
    .Request()
    .GetAsync();

```