---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67f717d0e60ed2462f952f5ef82d0998be478378d36696a182fd472c532224ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkAGI1AAAoZCfHAAA=')
    .version('beta')
    .get();

```