---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b32ffa5a3b7a2e0916b196e363b1c729fd8057d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "39843828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateRecordingStatusOperation = {
  clientContext: "clientContext-value",
  status: "notRecording | recording | failed"
};

let res = await client.api('/communications/calls/{id}/updateRecordingStatus')
    .version('beta')
    .post(updateRecordingStatusOperation);

```