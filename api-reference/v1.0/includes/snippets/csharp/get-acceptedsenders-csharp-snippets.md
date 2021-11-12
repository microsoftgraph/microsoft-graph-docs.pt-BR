---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d384f9bfd22e967c33ff6342725cd06a4cf993348eb674c333c84008ee7add5f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899312"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var acceptedSenders = await graphClient.Groups["{group-id}"].AcceptedSenders
    .Request()
    .GetAsync();

```