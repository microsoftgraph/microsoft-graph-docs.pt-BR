---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1836c0075f3a7c3e0d6b026480ca15348cc65c2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateProperties = {
  entityType: "Group",
  displayName: "Myprefix_test_mysuffix",
  mailNickname: "Myprefix_test_mysuffix",
  onBehalfOfUserId: "onBehalfOfUserId-value"
};

let res = await client.api('/directoryObjects/validateProperties')
    .version('beta')
    .post(validateProperties);

```