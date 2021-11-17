---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9faaa4ae24f029240f505bb284c31de371ecfa83ab14a24618503dd6a3d687e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272353"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var legalHold = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"]
    .Request()
    .GetAsync();

```