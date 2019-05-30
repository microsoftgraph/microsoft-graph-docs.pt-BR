---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba61ab57137b0c050ee11de6ebbc3b9db8ec6115
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites?search=%7Bquery%7D')
    .version('beta')
    .get();

```