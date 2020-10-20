---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7312921fb54a9fe579bb6e29c758323e27bc3a96
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608288"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/tiIndicators')
    .version('beta')
    .get();

```