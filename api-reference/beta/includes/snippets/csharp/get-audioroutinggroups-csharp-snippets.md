---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a45c0149bb9fe720b3226c20b9c32257b0927837
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302683"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroups = await graphClient.Communications.Calls["{id}"].AudioRoutingGroups
    .Request()
    .GetAsync();

```