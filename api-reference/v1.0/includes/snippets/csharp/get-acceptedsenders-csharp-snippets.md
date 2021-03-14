---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 272ce5792f227d81acf6d04d979f8cc485c720a5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792009"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var acceptedSenders = await graphClient.Groups["{group-id}"].AcceptedSenders
    .Request()
    .GetAsync();

```