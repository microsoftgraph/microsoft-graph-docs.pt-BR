---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56cd7959b9af10cce5f2443d8c5c7db11e501028394cbd752ba23ffa18159040
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'edit',
  scope: 'organization'
};

await client.api('/me/drive/items/{item-id}/createLink')
    .version('beta')
    .post(permission);

```