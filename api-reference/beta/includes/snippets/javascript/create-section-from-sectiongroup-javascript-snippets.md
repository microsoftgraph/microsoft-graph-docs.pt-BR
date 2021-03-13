---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1f4961bafa165e4185c81439dfef5aedf321864
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: 'Section name'
};

await client.api('/me/onenote/sectionGroups/{id}/sections')
    .version('beta')
    .post(onenoteSection);

```