---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9fcd2079b1c858a21d27a348685a978cbfecad45d2c167cd63a5044abacec93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{device-id}"].RegisteredOwners["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```