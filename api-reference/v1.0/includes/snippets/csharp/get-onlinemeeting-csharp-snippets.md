---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eca3dbe622e402ed16fd4c68f66f0bf7cccdcc80
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865673"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeetings = await graphClient.Communications.OnlineMeetings
    .Request()
    .Filter("VideoTeleconferenceId eq '123456789'")
    .GetAsync();

```