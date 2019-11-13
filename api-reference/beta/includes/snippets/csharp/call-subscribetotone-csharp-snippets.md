---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5994be4c43b2c66ea3a84e5ea50cde9eba5c819a
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302857"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54";

await graphClient.Communications.Calls["{id}"]
    .SubscribeToTone(clientContext)
    .Request()
    .PostAsync();

```