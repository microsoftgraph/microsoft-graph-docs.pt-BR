---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1836c0075f3a7c3e0d6b026480ca15348cc65c2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604987"
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