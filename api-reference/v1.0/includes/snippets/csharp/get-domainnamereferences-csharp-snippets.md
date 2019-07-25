---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4120044b5e0f277a9406057b813214174ff8cfc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733461"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domainNameReferences = await graphClient.Domains["{domain-name}"].DomainNameReferences
    .Request()
    .GetAsync();

```