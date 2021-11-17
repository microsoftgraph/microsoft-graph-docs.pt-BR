---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1826d8dd05c2a6c77aa711b256395afe005284736192c9dd61806f66955d132
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Projects["{projectParticipation-id}"]
    .Request()
    .DeleteAsync();

```