---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af98064b6d8d0b45bb435863beafff942ac52716
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11023')
    .version('beta')
    .get();

```