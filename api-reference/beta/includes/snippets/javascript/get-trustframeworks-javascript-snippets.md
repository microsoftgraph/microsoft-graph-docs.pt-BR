---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2b54fa9031b53d87b845627a049b9245df17471580d8659476958695459398ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let policies = await client.api('/trustFramework/policies')
    .version('beta')
    .get();

```