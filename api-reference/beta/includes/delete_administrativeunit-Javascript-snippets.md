---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b1e2d4aa138ffc0cece092808ee757e88c75819
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits/{id}')
    .version('beta')
    .delete();

```