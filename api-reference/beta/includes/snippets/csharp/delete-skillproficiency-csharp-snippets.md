---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29c2c86319f2dfca60064a7120ae265c82cbb8e7fcac4c86ed8eb73de4d21ff3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274870"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Skills["{skillProficiency-id}"]
    .Request()
    .DeleteAsync();

```