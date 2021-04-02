---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 881f159421f74f92667ccd43b2bd5686d131b840
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.TermStore.Groups["{termStore.group-id}"]
    .Request()
    .GetAsync();

```