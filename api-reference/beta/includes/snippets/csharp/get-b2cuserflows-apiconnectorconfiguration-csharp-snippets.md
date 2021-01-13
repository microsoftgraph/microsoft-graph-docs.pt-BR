---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f49a6d9e8eeccdebd42a576966ddbd6e59217719
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cUserFlows = await graphClient.Identity.B2cUserFlows["B2C_1_testuserflow"]
    .Request()
    .Expand("postAttributeCollection")
    .Select("ApiConnectorConfiguration")
    .GetAsync();

var apiConnectorConfiguration = b2cUserFlows.ApiConnectorConfiguration;

```