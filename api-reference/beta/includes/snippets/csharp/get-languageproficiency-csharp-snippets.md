---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92a0436a0b494e61c1a6940f0aad931174ac0342c984a0703a624cf001acd519
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100054"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = await graphClient.Me.Profile.Languages["{languageProficiency-id}"]
    .Request()
    .GetAsync();

```