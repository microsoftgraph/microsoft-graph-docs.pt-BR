---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9d806d91c7aebe962b1a5e125f0a3dd38fe577d0b274cc47b8f08130da66472
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].OverridesPages["{userFlowLanguagePage-id}"].Content
    .Request()
    .DeleteAsync();

```