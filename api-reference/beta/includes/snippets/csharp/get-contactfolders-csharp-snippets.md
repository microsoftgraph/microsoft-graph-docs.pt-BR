---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1b15df1afa9e870eb6291109af2e1c7dbfeb8ee
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolders = await graphClient.Me.ContactFolders
    .Request()
    .GetAsync();

```