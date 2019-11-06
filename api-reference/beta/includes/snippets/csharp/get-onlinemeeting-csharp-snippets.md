---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eca3dbe622e402ed16fd4c68f66f0bf7cccdcc80
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998210"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeetings = await graphClient.Communications.OnlineMeetings
    .Request()
    .Filter("VideoTeleconferenceId eq '123456789'")
    .GetAsync();

```