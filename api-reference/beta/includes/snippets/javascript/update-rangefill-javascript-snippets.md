---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 908090f634b19b2a9babc15318eb96ebd3e7b170
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796966"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: 'color-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .version('beta')
    .update(workbookRangeFill);

```