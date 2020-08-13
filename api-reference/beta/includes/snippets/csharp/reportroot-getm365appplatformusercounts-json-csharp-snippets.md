---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3369b093a2cf8792be54e46423cd70dd0099699
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2020
ms.locfileid: "46657961"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Reports
    .GetM365AppPlatformUserCounts("D7").Content
    .Request()
    .GetAsync();

```