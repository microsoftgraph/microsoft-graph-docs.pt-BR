---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a0d02e2ff63f785db2fb981a128505540e20a6a
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

var status = RecordingStatus.NotRecording | RecordingStatus.Recording | RecordingStatus.Failed;

await graphClient.Communications.Calls["{id}"]
    .UpdateRecordingStatus(status,clientContext)
    .Request()
    .PostAsync();

```