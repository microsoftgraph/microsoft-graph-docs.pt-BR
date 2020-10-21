---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22e9e161db499230e238f2a8b8bc325922b1e0ab
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rejectedSenders = await graphClient.Groups["{id}"].RejectedSenders
    .Request()
    .GetAsync();

```