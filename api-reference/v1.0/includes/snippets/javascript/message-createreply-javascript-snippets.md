---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cef3c7259a9c7745fb299f7d82d321b614eb6b6c0516059db286c99416f1ec03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/createReply')
    .post();

```