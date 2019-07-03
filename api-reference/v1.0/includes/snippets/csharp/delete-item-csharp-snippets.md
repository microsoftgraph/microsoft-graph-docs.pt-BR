---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94fcf705ef40e5070a8efcdee82e99b4d0b1c680
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .DeleteAsync();

```