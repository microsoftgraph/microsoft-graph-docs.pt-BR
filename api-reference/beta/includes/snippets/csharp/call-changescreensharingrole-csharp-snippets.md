---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 734e9bcfe77c82f5e67e9903567314dcea0a4da3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517834"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var role = ScreenSharingRole.Viewer;

await graphClient.App.Calls["{id}"]
    .ChangeScreenSharingRole(role)
    .Request()
    .PostAsync();

```