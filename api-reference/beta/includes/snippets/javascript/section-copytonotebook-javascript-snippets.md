---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7493e2ee1d36a3d7defa8113663fdb32cbe3850b05b380235f28d1aefd1ca85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214512"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: 'id-value',
  groupId: 'groupId-value',
  renameAs: 'renameAs-value'
};

await client.api('/me/onenote/sections/{id}/copyToNotebook')
    .version('beta')
    .post(onenoteOperation);

```