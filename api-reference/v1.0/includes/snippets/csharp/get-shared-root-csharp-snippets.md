---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8641e4da6e451a496f76b78081780270c8e261339e13139133102285c826154
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedDriveItem = await graphClient.Shares["{sharedDriveItem-id}"]
    .Request()
    .GetAsync();

```