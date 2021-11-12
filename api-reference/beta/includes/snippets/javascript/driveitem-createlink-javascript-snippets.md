---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 837c4f07e32b62a0ffbc7cd9cc7f616a8196c5352077134202ee7856c5a235c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'view',
  scope: 'anonymous',
  password: 'String',
  recipients: [
    {
      '@odata.type': 'microsoft.graph.driveRecipient'
    }
  ]
};

await client.api('/me/drive/items/{itemId}/createLink')
    .version('beta')
    .post(permission);

```