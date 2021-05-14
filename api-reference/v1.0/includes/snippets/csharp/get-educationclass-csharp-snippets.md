---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c053af0ee2efee9f170d6004ea3dae08a0997a03
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52474985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = await graphClient.Education.Classes["{educationClass-id}"]
    .Request()
    .GetAsync();

```