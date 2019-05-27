---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a523035e3b4778a6529fb35a785c3579d4c4ec54
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435897"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants')
    .version('beta')
    .header('Authorization','Bearer <TOKEN>')
    .get();

```