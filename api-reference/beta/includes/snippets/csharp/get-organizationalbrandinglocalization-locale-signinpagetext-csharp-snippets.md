---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 091d758e31f7f31e3c90c1c48eba85b370c14cd1
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996802"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var localizations = await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"]
    .Request()
    .Select("SignInPageText")
    .GetAsync();

var signInPageText = localizations.SignInPageText;

```