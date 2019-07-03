---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0edb733a5f4084042f85fca2f0307955033d3f18
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataPolicyOperation = await graphClient.DataPolicyOperations["{id}"]
    .Request()
    .GetAsync();

```