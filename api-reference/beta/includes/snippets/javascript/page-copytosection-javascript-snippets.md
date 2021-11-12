---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ed42143b98540ca4c0fb8184a174b618f9075f2eb14d8d1f2acb299e0844d97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273697"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: 'id-value',
  groupId: 'groupId-value'
};

await client.api('/me/onenote/pages/{id}/copyToSection')
    .version('beta')
    .post(onenoteOperation);

```