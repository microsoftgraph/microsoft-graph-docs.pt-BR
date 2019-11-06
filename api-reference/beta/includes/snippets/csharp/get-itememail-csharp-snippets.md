---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 252b799f672b1994627b98bcf8c843a34c7e5a14
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemEmail = await graphClient.Me.Profile.Emails["{id}"]
    .Request()
    .GetAsync();

```