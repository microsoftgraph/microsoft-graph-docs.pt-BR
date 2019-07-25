---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8e7b57fd79cbe7fd484584ccbdd97c53068e694
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .GetAsync();

```