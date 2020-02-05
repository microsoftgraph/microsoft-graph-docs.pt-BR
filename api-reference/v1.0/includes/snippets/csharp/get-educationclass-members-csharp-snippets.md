---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04fb7e3f14aa5338135af2f3b087024542bf1d0d
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Education.Classes["{class-id}"].Members
    .Request()
    .GetAsync();

```