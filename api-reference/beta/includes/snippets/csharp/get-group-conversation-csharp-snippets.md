---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1a7084effc441b88a9f0e216ba7701061872458c54ba72e6d32d845239a5833
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"]
    .Request()
    .GetAsync();

```