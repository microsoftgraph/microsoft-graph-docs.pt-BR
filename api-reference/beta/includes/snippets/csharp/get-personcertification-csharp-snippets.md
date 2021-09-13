---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc57d5b96491b794d1daec2398c2674ecb6e9d4c3e6a009584ddeeceeaf5a091
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personCertification = await graphClient.Me.Profile.Certifications["{personCertification-id}"]
    .Request()
    .GetAsync();

```