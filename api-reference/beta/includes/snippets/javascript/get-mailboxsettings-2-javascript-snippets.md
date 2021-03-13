---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7da7e9611f8dd034b0226f0d6a9a5410472fd2bc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let automaticRepliesSetting = await client.api('/me/mailboxSettings/automaticRepliesSetting')
    .version('beta')
    .get();

```