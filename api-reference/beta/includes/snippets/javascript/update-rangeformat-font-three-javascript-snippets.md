---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71e7a27d614300606bca058386cb25efa7bce35a822b226520c13fd11316346a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  underline: 'Single',
  color: '#FFFFFF',
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font')
    .version('beta')
    .update(workbookRangeFont);

```