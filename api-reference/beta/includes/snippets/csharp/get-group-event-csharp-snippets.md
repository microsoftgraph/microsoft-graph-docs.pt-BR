---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 099fab61a27157c9e0c01d051cb72327b989c5c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797223"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Groups["{group-id}"].Events["{event-id}"]
    .Request()
    .GetAsync();

```