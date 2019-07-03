---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d35797e52c3b516d0318a9206b22361f4e1cf95a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/{id}/childFolders')
    .post({mailFolder : mailFolder});

```