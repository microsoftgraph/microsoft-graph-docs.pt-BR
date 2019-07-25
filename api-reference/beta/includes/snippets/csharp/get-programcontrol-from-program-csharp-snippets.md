---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 120a81d6af6929de65aa7ef5b021e795fe578f89
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var controls = await graphClient.Programs["673a7379-9c38-4f01-bd9d-4fda7260b807"].Controls
    .Request()
    .GetAsync();

```