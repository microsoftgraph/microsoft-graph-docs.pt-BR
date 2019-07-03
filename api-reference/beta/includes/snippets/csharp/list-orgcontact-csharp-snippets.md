---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 235b7a0e8a8fa24c2dcc19fe790f44b7a4292abe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476260"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .GetAsync();

```