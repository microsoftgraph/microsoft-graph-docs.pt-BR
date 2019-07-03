---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5362a54b861ab76cafe4ad723052e2e31ae7b176
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var posts = await graphClient.Groups["0d75b8dc-c42d-44dd-890a-751a99c0589f"].Threads["AAQkAD8EJUmcWwTJi06Cew=="].Posts
    .Request()
    .GetAsync();

```