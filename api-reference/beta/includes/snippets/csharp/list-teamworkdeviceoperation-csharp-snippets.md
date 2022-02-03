---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d10524eca3bdfb96857182b2e0f38036648b6787
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Teamwork.Devices["{teamworkDevice-id}"].Operations
    .Request()
    .GetAsync();

```