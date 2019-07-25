---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de6074e17bad718fe062b5a535d8120a39fd3056
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861278"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root
    .Delta()
    .Request()
    .GetAsync();

```