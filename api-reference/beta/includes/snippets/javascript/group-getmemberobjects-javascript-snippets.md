---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbd33adb6f0968a7c82a0d911bb562a07f952351
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberObjects')
    .version('beta')
    .post(string);

```