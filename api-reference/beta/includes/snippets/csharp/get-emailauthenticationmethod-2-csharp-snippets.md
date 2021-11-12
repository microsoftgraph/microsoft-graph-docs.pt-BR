---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52a6084589abda6cf0bcfb5c3486685ee35f3964fe2eeb2431c61cb51debd982
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102878"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailMethods = await graphClient.Me.Authentication.EmailMethods
    .Request()
    .GetAsync();

```