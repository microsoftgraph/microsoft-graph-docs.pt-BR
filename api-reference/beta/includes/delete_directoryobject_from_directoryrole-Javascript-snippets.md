---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2732d023798b4af955503939406d485fd104fef7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryroles/{id}/members/{id}/$ref')
    .version('beta')
    .delete();

```