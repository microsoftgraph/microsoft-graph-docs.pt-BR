---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1a7a3b552d63f83fdc7f34ff2ec15a3c92120e92ce2677e1b089df7faa36b16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

var status = RecordingStatus.NotRecording | RecordingStatus.Recording | RecordingStatus.Failed;

await graphClient.Communications.Calls["{call-id}"]
    .UpdateRecordingStatus(status,clientContext)
    .Request()
    .PostAsync();

```