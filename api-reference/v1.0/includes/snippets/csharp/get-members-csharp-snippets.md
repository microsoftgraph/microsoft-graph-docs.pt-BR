---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87ea6a9955decfca7ce6cadec6c4e5b1c3e6e45d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Groups["{id}"].Members
    .Request()
    .GetAsync();

```