---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e092ecffd01da1a5f95dc10b99d4a75e3d663e90
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/usedRange')
    .get();

```