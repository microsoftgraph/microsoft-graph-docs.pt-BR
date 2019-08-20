---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 652659b3ae7eec1f544e974e30d9913532e32147
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36464972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscribeToToneOperation = {
  clientContext: "fd1c7836-4d84-4e24-b6aa-23188688cc54"
};

let res = await client.api('/app/calls/{id}/subscribeToTone')
    .version('beta')
    .post(subscribeToToneOperation);

```