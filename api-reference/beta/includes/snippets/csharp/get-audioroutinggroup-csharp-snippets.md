---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daf98a78e3fad144c8158810265ad5773923a1060f7d9c4c7a2513fd36f82f05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100193"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroup = await graphClient.Communications.Calls["{call-id}"].AudioRoutingGroups["{audioRoutingGroup-id}"]
    .Request()
    .GetAsync();

```