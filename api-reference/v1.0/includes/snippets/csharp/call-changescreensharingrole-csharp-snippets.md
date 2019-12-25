---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36a8337d2658bddd7c29ebc3e1344bcd530f5429
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var role = ScreenSharingRole.Viewer;

await graphClient.Communications.Calls["{id}"]
    .ChangeScreenSharingRole(role)
    .Request()
    .PostAsync();

```