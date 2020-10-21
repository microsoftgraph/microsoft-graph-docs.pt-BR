---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4120044b5e0f277a9406057b813214174ff8cfc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606525"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domainNameReferences = await graphClient.Domains["{domain-name}"].DomainNameReferences
    .Request()
    .GetAsync();

```