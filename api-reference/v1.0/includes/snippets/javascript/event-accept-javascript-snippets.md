---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 385ab7627258b6b86c1f86b4d2884585fc3def8f56769f55eaea3e7aee54d891
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327540"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accept = {
  comment: 'comment-value',
  sendResponse: true
};

await client.api('/me/events/{id}/accept')
    .post(accept);

```