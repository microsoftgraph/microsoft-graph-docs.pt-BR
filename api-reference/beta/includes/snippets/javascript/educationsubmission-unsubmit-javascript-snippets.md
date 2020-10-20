---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f688422c886ad4589068bd971f24f11e3942bc7b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614443"
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