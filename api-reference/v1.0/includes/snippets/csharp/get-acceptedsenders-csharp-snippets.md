---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0176e4d9dc5b10f6b75a7a987d16e6f7cc32d54
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var acceptedSenders = await graphClient.Groups["{id}"].AcceptedSenders
    .Request()
    .GetAsync();

```