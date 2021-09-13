---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 189e1a36bf52968fa76445d1563d59a377a67385c66f814890b8c8483a07397d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkBot = await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"].AppDefinitions["{teamsAppDefinition-id}"].Bot
    .Request()
    .GetAsync();

```