---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a59ec5670ed04332b49d771cb530815a37b92d4b5c4dee55bbf28b842cd747b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = await graphClient.Places["{place-id}"]
    .Request()
    .GetAsync();

```