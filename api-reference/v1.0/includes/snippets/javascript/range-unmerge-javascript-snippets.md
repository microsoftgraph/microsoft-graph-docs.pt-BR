---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6ff534214be8f2865ba269a698d48cff464f754
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/unmerge')
    .post();

```