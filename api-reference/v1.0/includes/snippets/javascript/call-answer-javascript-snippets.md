---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1df565b9d2fd0b82bef5bb4507ca02e5a84daea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: "callbackUri-value",
  mediaConfig: {
    @odata.type: "#microsoft.graph.appHostedMediaConfig",
    blob: "<Media Session Configuration Blob>"
  },
  acceptedModalities: [
    "audio"
  ]
};

let res = await client.api('/communications/calls/{id}/answer')
    .post(answer);

```