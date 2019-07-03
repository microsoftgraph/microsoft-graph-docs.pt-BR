---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6bd4665a76282fe1e553b2f9e1255d0358b0eef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope,expirationDateTime,password,message,recipients)
    .Request()
    .PostAsync();

```