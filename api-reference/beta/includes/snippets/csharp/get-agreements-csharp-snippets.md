---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81cb511d07cb9f8079cc625eb4aab928c0ff0c6e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreements = await graphClient.Agreements
    .Request()
    .GetAsync();

```