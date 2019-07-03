---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e092ecffd01da1a5f95dc10b99d4a75e3d663e90
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/usedRange')
    .get();

```