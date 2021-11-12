---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6421e618d82d177d61e47d1c9f3946bce7214e4d1729145a90138a064a9a3044
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/education/users')
    .version('beta')
    .get();

```