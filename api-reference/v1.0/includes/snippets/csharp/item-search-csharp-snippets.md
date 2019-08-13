---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a71e46120d5a73160648acb9f43449350ae7627c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367233"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Root
    .Search("{search-query}")
    .Request()
    .GetAsync();

```