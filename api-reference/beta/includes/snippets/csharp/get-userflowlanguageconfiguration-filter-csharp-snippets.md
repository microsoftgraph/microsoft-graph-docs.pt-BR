---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94cc3525beffdac69ef2051489b70b0355ed39fa
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844087"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2cUserFlows["B2C_1_CustomerSignUp"].Languages
    .Request()
    .Filter("isEnabled eq true")
    .GetAsync();

```