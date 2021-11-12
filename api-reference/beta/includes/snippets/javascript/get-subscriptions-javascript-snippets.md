---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e804d8185557ff390eafa21b8b73ec5e82366ebd7497224b01b1ff4014c89d46
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329648"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscriptions = await client.api('/subscriptions')
    .version('beta')
    .get();

```