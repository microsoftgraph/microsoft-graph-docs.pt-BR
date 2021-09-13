---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d438cfbd60bbf2a5b4d320ce8bdaecd7119e360dff8e9b00259c9db14f66e2b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setSolidColor = {
  color: 'color-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor')
    .post(setSolidColor);

```