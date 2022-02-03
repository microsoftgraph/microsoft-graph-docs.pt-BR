---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50a75c77440592e005ab066d3ea6d913ea865d78
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Teamwork.Devices
    .Request()
    .GetAsync();

```