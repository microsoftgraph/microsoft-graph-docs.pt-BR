---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f28e13e5d931c4929d1d0ce21a54538dc8bae5fc
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Classes["11014"].Schools
    .Request()
    .GetAsync();

```