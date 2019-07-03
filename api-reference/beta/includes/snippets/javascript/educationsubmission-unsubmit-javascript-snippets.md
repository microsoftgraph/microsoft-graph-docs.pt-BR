---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f688422c886ad4589068bd971f24f11e3942bc7b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit')
    .version('beta')
    .post();

```