---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f96a2bf18b83d84528759146a4a6b560fe7630c3
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "47414043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/directoryObjects/{id}"
};

let res = await client.api('/groups/{group-id}/members/$ref')
    .version('beta')
    .post(directoryObject);

```