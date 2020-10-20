---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8359efd783dbc4ae323b1ebf398e2f8959a2e3bd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/registeredDevices')
    .version('beta')
    .get();

```