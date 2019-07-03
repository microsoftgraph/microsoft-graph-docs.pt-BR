---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0933b3bcf9bdabc4026ba9a9c4c05d530e799dda
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517586"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["10002"]
    .Request()
    .DeleteAsync();

```