---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdd40850409273d2ebb0882fb4cc3c92323c83f1
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = await graphClient.Communications.Calls["2f1a1100-b174-40a0-aba7-0b405e01ed92"]
    .Request()
    .GetAsync();

```