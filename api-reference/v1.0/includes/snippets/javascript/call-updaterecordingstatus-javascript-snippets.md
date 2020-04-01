---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3ddfdd2a6fa6f4153ff70fded55d29790804ed7
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082279"
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
    .post(updateRecordingStatusOperation);

```