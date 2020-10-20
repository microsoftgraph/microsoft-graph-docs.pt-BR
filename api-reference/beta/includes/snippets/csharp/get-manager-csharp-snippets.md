---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35d0af3bfa42f85c0b5ab350895a99f7b49d6ab9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Contacts["{id}"].Manager
    .Request()
    .GetAsync();

```