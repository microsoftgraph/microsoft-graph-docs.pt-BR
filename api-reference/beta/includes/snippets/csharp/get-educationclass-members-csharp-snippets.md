---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 900ffa40398aae5aee9592ff9d76bf2178aa98f2
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774393"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Education.Classes["11016"].Members
    .Request()
    .GetAsync();

```