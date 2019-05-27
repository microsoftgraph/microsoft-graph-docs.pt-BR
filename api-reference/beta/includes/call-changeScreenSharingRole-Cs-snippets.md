---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03ac8216c6e7c9f1e9aa209921edab4074045f90
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var role = "viewer";

await graphClient.App.Calls["{id}"]
    .ChangeScreenSharingRole(role)
    .Request()
    .PostAsync();

```