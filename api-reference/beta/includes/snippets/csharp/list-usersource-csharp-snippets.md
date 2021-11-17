---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c81cba24aed2870d0ce565d00d8dfa0f2ba6625fbf4d8fba97820350fffc9c73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"].UserSources
    .Request()
    .GetAsync();

```