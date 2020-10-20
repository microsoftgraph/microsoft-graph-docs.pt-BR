---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de0889463eaf7183573ac40e2e237b9aa65fe5fa
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/rejectedSenders')
    .version('beta')
    .get();

```