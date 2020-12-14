---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3107fb10b9cba534c9cbb157e968dd556d5ef4e
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodians = await graphClient.Compliance.Ediscovery.Cases["2192ca408ea2410eba3bec8ae873be6b"].Custodians
    .Request()
    .GetAsync();

```