---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af518bf1ab80fdf6ee3a6bf86b3b96fa88d5dd6d
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "35732107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  comment: "comment-value",
  toRecipients: [
    {
      emailAddress: {
        name: "name-value",
        address: "address-value"
      }
    }
  ]
};

let res = await client.api('/me/messages/{id}/forward')
    .post(forward);

```