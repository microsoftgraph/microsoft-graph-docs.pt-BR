---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bac6ea6efca9ef93f3a94e6055f55adabdce3c0a
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610834"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .GetAsync();

```