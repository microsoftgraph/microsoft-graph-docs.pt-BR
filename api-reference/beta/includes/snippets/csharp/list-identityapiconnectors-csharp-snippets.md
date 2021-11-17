---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5dceb3eb292365206cc8c1a0edde1cf739526edcef91248e620fc36f727de446
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100055"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var apiConnectors = await graphClient.Identity.ApiConnectors
    .Request()
    .GetAsync();

```