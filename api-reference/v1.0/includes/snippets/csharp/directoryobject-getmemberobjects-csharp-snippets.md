---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 939dafdfa2983ee68ebb771a3b75a8d3bb465a08
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.DirectoryObjects["{object-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```