---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d09f1998c8932f043b13b841aad423323bbe1b82
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11014/assignments/19002')
    .version('beta')
    .delete();

```