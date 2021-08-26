---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d37f92bb46f80b0fcfc14e2f9da413966f98b100d90fa0e88381ab93bb6d2cff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327356"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.Messages["{message-id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```