---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 844c3ccabc2e302d77ef8a8149823a68d552fab4
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680903"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/authenticationFlowsPolicy')
    .version('beta')
    .get();

```