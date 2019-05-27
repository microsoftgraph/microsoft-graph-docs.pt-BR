---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3207cc4709ebc0c17ad8d003ab205c8486df1a8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438452"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/resources/22002')
    .version('beta')
    .delete();

```