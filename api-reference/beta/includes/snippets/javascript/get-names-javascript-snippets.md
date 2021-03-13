---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ac24e9c0e76ac104478d7898129dd7196af7c23
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794262"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/profile/names')
    .version('beta')
    .get();

```