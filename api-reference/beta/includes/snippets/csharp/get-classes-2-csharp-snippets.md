---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddeb2961b5bac169cbc8a46cb5cce6414c6ce8ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951323"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Schools["{educationSchool-id}"].Classes
    .Request()
    .GetAsync();

```