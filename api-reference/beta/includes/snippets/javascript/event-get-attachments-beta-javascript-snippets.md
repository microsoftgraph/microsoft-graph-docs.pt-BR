---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc74b999c98ec8e09cb12bf00f1052bf9f9d94c938c2dbe885041bdf856f1f95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/me/events/{id}/attachments')
    .version('beta')
    .get();

```