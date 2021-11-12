---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36a5ad1a203f6f898c65748301714788c18858639cb5a9bfeaf16b0c8845ad06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,null,null,null,null,null)
    .Request()
    .PostAsync();

```