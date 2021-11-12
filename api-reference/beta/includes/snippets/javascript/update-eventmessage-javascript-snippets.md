---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee2e7da5845db5abfa94e758fed79f31fec070abdb7822760d8e1f41c5a65cbc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: 'true',
};

await client.api('/me/messages/{id}')
    .version('beta')
    .update(message);

```