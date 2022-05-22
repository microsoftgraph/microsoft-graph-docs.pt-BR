---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2867f23fb607bc0da78c15c33d0ee76128d76714
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = await graphClient.Groups["{group-id}"].Settings["{groupSetting-id}"]
    .Request()
    .GetAsync();

```