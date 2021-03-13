---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 281a268f4e944c3c985f034b0baae3bf36c3597a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateProperties = {
  entityType: 'Group',
  displayName: 'Myprefix_test_mysuffix',
  mailNickname: 'Myprefix_test_mysuffix',
  onBehalfOfUserId: 'onBehalfOfUserId-value'
};

await client.api('/directoryObjects/validateProperties')
    .version('beta')
    .post(validateProperties);

```