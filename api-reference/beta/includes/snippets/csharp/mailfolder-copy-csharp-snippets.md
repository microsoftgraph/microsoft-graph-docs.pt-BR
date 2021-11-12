---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 598ceec42fce5d5ade7ecb28a730a2b66f84189879a55b0a02dd63d192405d0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```