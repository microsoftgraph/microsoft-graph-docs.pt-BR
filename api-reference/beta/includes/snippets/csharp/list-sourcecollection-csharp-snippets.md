---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8f85d8d6198e280dd86821acc0ecdb9f6bd5c6bb9d0462010137717e975b131
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327205"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollections = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections
    .Request()
    .GetAsync();

```