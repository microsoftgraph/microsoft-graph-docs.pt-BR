---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 254965554b9c8d790bad85ac9cccf10d2303c011
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var richLongRunningOperation = await graphClient.Sites["{site-id}"].Operations["{richLongRunningOperation-id}"]
    .Request()
    .GetAsync();

```