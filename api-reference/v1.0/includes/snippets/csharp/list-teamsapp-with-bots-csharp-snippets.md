---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 495b2e20e78c11fa715d322557b4632d03224aa8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774849"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("appDefinitions/any(a:a/bot ne null)")
    .Expand("appDefinitions($expand=bot)")
    .GetAsync();

```