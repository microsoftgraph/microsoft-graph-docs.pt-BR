---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 846010e5b6a06f566dc6fc405496ad71fabebd3808f401a4229d0aaed925c64b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  type: 'type-value',
  scope: 'scope-value',
  comment: 'comment-value',
  value: {
  },
  visible: true
};

await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .update(workbookNamedItem);

```