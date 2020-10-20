---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abaae7631defb1fb4d1526be6f09ada2cdb61cb2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/agreementAcceptances')
    .version('beta')
    .get();

```