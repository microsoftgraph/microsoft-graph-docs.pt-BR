---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7948c093c672d2c4d2c02a2aca4fe007a81531ae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "fee2c45b-915a-4a64b130f4eb9e75525e",
    "4fe90ae065a-478b9400e0a0e1cbd540"
};

await graphClient.DirectoryObjects["{id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```