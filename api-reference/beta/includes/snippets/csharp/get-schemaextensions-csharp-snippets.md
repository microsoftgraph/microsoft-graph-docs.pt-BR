---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d5e88b8a65a35e21615eba492ad5cb6b6e5c1a2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtensions = await graphClient.SchemaExtensions
    .Request()
    .Filter("id eq 'graphlearn_test'")
    .GetAsync();

```