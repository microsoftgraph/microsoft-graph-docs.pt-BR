---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bace61dfa92f0a4765d15e79e7d18fd35e9f953f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = [
   {
    \'target\':\'#para-id\',
    \'action\':\'insert\',
    \'position\':\'before\',
    \'content\':\'<img src='image-url-or-part-name' alt='image-alt-text' />\'
  }, 
  {
    \'target\':\'#list-id\',
    \'action\':\'append\',
    \'content\':\'<li>new-page-content</li>\'
  }
];

await client.api('/me/onenote/pages/{id}/content')
    .version('beta')
    .update(stream);

```