---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 175aa306b8ef90b2e551ab2d9b3c6ffd87ec8a13
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  members@odata.bind: [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
};

let res = await client.api('/groups/{group-id}')
    .update(group);

```