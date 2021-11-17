---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8396d9f8b0ac33e644582df47822867e0f29d786136e533118baa6961254ac60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157284"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Items["{driveItem-id}"]
    .Request()
    .DeleteAsync();

```