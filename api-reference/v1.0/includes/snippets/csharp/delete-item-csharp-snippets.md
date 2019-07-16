---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94fcf705ef40e5070a8efcdee82e99b4d0b1c680
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .DeleteAsync();

```