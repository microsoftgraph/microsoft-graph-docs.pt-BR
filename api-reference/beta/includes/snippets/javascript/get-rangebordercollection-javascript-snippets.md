---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb248bd577ecff827ac2d2bc8d766ae72d917d2a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders')
    .version('beta')
    .get();

```