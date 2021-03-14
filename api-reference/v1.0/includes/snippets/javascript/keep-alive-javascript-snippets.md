---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8a1f4767886a878d358f92d02d39bbbe7ff9025
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive')
    .post();

```