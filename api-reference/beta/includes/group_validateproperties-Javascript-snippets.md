---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 246b574f64b1f4a450134547e046673c50cb0ee0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444612"
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