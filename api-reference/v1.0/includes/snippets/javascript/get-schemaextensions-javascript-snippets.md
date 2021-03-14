---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcbcafc6f9ccdb29cd82ed144c0f4b12ca977faa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798174"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schemaExtensions = await client.api('/schemaExtensions')
    .filter('id eq \'graphlearn_test\'')
    .get();

```