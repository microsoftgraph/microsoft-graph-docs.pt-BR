---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3fd61b5c5b7586c31cb253e235021f901bf7c427c337f603ebdc4481353b5097
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213723"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var storageLocation = "storageLocation-value";

await graphClient.Users["{user-id}"]
    .ExportPersonalData(storageLocation)
    .Request()
    .PostAsync();

```