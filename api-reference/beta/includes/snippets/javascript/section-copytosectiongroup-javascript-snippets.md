---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74055a669d4503c0679e0d822979803888dd6923f19c07330c0d30f062b5791a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099622"
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

await client.api('/me/onenote/sections/{id}/copyToSectionGroup')
    .version('beta')
    .post(onenoteOperation);

```