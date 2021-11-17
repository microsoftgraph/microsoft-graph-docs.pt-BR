---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a11fa35726fe926988b7232e6d3a2bcd0b352d7efac6f38b31b8b588ee360a74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100934"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Calendar
    .Request()
    .DeleteAsync();

```