---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e844b7aa819c6db68bb130e4dee448029e6f8eaf
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48907375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: true,
};

let res = await client.api('/me/messages/{id}')
    .update(message);

```