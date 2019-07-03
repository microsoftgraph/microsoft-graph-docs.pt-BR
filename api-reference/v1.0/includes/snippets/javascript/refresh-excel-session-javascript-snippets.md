---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f74bb9512041406fdb5a6506b24e0d9cd0a39845
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508613"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const refreshSession = {

};

let res = await client.api('/me/drive/items/{id}/workbook/refreshSession')
    .post(refreshSession);

```