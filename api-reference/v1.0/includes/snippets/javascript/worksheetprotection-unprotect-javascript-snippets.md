---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f423c9caa5a9d0c99343e8e77cd8ef7140cf1d59
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unprotect = {
  password: 'password-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect')
    .post(unprotect);

```