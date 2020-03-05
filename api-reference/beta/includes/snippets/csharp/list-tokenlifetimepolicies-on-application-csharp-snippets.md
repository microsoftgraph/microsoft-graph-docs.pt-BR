---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2ad2885ec036baab103ed1c09f120acaa81eb4f
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicies = await graphClient.Applications["{id}"].TokenLifetimePolicies
    .Request()
    .GetAsync();

```