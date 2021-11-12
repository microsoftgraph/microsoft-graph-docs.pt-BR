---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dee927951c682df666d72b85f3b177d67e7dba3b5c716dd365328ac44cc4d88c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AQMkADJmMTUAAAgVZAAAA/')
    .version('beta')
    .expand('mentions')
    .get();

```