---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 246b574f64b1f4a450134547e046673c50cb0ee0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateProperties = {
  displayName: "Myprefix_test_mysuffix",
  mailNickname: "Myprefix_test_mysuffix",
  onBehalfOfUserId: "onBehalfOfUserId-value"
};

let res = await client.api('/groups/{id}/validateProperties')
    .version('beta')
    .post(validateProperties);

```