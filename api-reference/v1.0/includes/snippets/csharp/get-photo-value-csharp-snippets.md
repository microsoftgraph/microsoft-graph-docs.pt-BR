---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01d5c5208d9af9bedba12ec9bc3fa810f42f0097
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Users["{id|userPrincipalName}"].Photo.Content
    .Request()
    .GetAsync();

```