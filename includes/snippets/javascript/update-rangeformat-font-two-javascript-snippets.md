---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10a6af6775ecc7adaf935250c9fb4a8b0d36979b14bd5ccced387ea7c3f6cfbb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  italic: true,
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font')
    .update(workbookRangeFont);

```