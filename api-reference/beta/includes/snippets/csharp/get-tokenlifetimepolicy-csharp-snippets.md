---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00f964ddb944480fa8ea59a925f23bd62df111c5
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var {id} = await graphClient.Policies["tokenLifetimePolicies"].{id}
    .Request()
    .GetAsync();

```