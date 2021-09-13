---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad769ced08cb889d520392f7cfa2698292ebdce2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columnDefinition = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"].Columns["{columnDefinition-id}"]
    .Request()
    .GetAsync();

```