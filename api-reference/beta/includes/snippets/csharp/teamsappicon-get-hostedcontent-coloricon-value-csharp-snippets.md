---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fdec94d01c41668dd7cf7016d6aad1920976e20f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921687"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkHostedContent = await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"].AppDefinitions["{teamsAppDefinition-id}"].ColorIcon.HostedContent
    .Request()
    .GetAsync();

```