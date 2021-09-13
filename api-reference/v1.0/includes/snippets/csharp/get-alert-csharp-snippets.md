---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 950902ce431b3db87d0f78e225578d37e9185e24cbfcdaecebab0fd43079a60a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{alert-id}"]
    .Request()
    .GetAsync();

```