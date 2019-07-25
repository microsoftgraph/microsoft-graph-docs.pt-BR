---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f93ebfc3c12d0b88fa77b53fe1eeeee2a94a3191
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Contacts["{id}"]
    .Request()
    .DeleteAsync();

```