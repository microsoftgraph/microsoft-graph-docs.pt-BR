---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 744d2b123705cba72bbb87a529591567f7d568d7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61076981"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .Select("displayName,givenName,postalCode,identities")
    .GetAsync();

```