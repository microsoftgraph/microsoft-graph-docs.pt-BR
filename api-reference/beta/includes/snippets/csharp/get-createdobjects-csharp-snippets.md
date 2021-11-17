---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96785a0baa926f0796bceb27b1e1ccf74aa466641fb45d8c25b47143d5bbb662
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var createdObjects = await graphClient.Me.CreatedObjects
    .Request()
    .GetAsync();

```