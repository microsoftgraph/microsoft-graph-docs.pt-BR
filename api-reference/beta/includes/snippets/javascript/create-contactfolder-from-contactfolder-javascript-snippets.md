---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c82f8b7c73f8d346113249be4c79a56b8ac88777
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .post({contactFolder : contactFolder});

```