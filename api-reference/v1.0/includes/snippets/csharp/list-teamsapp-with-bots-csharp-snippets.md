---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d68c4e5c9b5ca5b01d46ef4e577e04f7a177655c7681a37624a4bb259ea3ed85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("appDefinitions/any(a:a/bot ne null)")
    .Expand("appDefinitions($expand=bot)")
    .GetAsync();

```