---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f29c292ead64a5879b8f27e0d0f00318d70094ac
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups')
    .version('beta')
    .get();

```