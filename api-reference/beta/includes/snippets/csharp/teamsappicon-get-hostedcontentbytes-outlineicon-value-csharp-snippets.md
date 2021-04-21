---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2efc275cc16450a2ecc034273052f635ccdb7c0e
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921684"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"].AppDefinitions["{teamsAppDefinition-id}"].OutlineIcon.HostedContent.Content
    .Request()
    .GetAsync();

```