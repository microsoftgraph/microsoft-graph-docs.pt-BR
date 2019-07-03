---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 161636dac4a8270b9693d1594bf25b3a9ba6b08a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/publish')
    .version('beta')
    .post();

```