---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0439f3d116b98e340665dc5fb8b8ab15480348ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/schools/10002/classes')
    .version('beta')
    .get();

```