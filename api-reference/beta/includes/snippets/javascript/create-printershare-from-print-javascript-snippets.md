---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a03bb70a06fe8903c05dbf6c3f861356ac68c316e69839535fa72aad3fa531cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  name: 'name-value',
  'printer@odata.bind': 'https://graph.microsoft.com/beta/print/printers/{id}'
};

await client.api('/print/shares')
    .version('beta')
    .post(printerShare);

```