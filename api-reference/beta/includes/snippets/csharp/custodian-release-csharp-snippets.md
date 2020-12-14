---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5953af3ffadb43d90cfb8150434dab7e398d1397
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["2192ca408ea2410eba3bec8ae873be6b"].Custodians["45454331323337443946343043464239"]
    .Release()
    .Request()
    .PostAsync();

```