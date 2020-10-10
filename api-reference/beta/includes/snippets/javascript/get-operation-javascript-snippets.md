---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a35ee56dc6602a084c985eda401e9ef502822f51
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id | userPrincipalName}/authentication/operations/{id}')
    .version('beta')
    .get();

```