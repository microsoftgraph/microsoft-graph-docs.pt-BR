---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15e8f1f739783669bb15b369c04aa017c61a8c2b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}')
    .get();

```