---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab9a054a39a564a71168c083b7903a83e9a720a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797735"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateProperties = {
  displayName: 'Myprefix_test_mysuffix',
  mailNickname: 'Myprefix_test_mysuffix',
  onBehalfOfUserId: 'onBehalfOfUserId-value'
};

await client.api('/groups/{id}/validateProperties')
    .version('beta')
    .post(validateProperties);

```