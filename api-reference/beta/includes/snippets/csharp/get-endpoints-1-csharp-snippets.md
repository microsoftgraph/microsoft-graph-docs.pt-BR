---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e030941d6077e8298389a3f5814de838b25bdb8c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoints = await graphClient.Groups["{group-id}"].Endpoints
    .Request()
    .GetAsync();

```