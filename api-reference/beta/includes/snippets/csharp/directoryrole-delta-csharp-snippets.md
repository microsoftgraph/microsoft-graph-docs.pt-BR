---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ef432fbe22b31ef2661884eaf4da20447d889f2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.DirectoryRoles.Delta()
    .Request()
    .GetAsync();

```