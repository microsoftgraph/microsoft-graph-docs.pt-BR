---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd84b402aa8d1de28f74e34b8b55619eb8f322af
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskDefinition = new PrintTaskDefinition
{
    DisplayName = "Test TaskDefinitionName",
    CreatedBy = new AppIdentity
    {
        DisplayName = "Requesting App Display Name"
    }
};

await graphClient.Print.TaskDefinitions["fab143fd-ee61-4358-8558-2c7dee953982"]
    .Request()
    .UpdateAsync(printTaskDefinition);

```