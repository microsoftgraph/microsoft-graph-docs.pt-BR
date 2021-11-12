---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edfb6eee453500863d0b37ac5fa0c931aed0287fe503552216f59f5242f80a4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214176"
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
    .version('beta')
    .post(accept);

```