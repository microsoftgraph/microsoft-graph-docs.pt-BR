---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bce7f3bfb34d02cd2c2d087544f8e38abf260774
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507623"
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