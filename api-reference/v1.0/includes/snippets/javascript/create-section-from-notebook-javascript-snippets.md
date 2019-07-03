---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc71407e30ba0bf8342b4f4023e5ddeba3179644
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: "Section name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sections')
    .post({onenoteSection : onenoteSection});

```