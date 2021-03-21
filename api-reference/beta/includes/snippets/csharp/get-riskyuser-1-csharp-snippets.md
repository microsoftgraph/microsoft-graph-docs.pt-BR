---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55b587fc56ed96995667db244ba7b276e4b6a556
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUser = await graphClient.RiskyUsers["{riskyUser-id}"]
    .Request()
    .GetAsync();

```