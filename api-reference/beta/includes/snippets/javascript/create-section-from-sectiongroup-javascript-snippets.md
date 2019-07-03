---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 052e68ff451e47635264acf4bf91cfaea7d08edf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477877"
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
    .version('beta')
    .post({onenoteSection : onenoteSection});

```