---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a24426d9157af105d70e63a007b2fcb8190f64f9
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266665"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAssets = await graphClient.Admin.Windows.Updates.UpdatableAssets
    .Request()
    .GetAsync();

```