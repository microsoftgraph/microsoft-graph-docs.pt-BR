---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bce7f3bfb34d02cd2c2d087544f8e38abf260774
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: "Section name"
};

let res = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .post({onenoteSection : onenoteSection});

```