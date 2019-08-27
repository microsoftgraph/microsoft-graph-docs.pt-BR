---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc8f44c4983f59417850dde6b8a271b1679487d6
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "Self help community for golf",
  displayName: "Golf Assist",
  groupTypes: [
    "Unified"
  ],
  mailEnabled: true,
  mailNickname: "golfassist",
  securityEnabled: false
};

let res = await client.api('/groups')
    .version('beta')
    .post(group);

```