---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f507495391958afd6fbac4339f161b3359bf384
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var localizations = await graphClient.Organization["d69179bf-f4a4-41a9-a9de-249c0f2efb1d"].Branding.Localizations["en-US"]
    .Request()
    .Select("SignInPageText")
    .GetAsync();

var signInPageText = localizations.SignInPageText;

```