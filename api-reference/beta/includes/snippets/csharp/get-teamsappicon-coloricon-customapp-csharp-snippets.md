---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc661bbc547a41e0c21bc7c0494a361ccf4db43ee91d1fe9f55fa66f900a806b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214482"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppIcon = await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"].AppDefinitions["{teamsAppDefinition-id}"].ColorIcon
    .Request()
    .GetAsync();

```