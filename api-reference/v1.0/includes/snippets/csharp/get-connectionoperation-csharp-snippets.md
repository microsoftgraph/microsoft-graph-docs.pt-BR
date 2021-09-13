---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0dc83f5a1af1a7472e075460b5dedc09b39d6d6bf45a4d0341ec20f6f2d73eaa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectionOperation = await graphClient.Connections["{externalConnectors.externalConnection-id}"].Operations["{externalConnectors.connectionOperation-id}"]
    .Request()
    .GetAsync();

```