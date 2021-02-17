---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8655cad4bc63e104b23668fe964deffaea29f5e
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274810"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSources = await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].SiteSources
    .Request()
    .GetAsync();

```