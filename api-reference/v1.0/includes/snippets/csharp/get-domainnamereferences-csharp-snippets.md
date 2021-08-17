---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b476bce0ab121cc4c6d4b0c1428ef63808a2ee89343bb691c37080461f3601e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domainNameReferences = await graphClient.Domains["{domain-id}"].DomainNameReferences
    .Request()
    .GetAsync();

```