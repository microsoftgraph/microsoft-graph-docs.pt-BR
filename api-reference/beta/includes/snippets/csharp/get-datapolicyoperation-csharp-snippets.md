---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0edb733a5f4084042f85fca2f0307955033d3f18
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataPolicyOperation = await graphClient.DataPolicyOperations["{id}"]
    .Request()
    .GetAsync();

```