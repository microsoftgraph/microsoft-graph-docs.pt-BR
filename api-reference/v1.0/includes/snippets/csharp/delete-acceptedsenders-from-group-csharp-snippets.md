---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7a1783b24ba6aff07bb471adfc0ac3119a0c8041850cb0b0a46c6f3fc262f9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274533"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].AcceptedSenders.References
    .Request()
    .DeleteAsync();

```