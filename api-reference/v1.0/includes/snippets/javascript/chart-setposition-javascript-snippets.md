---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0132d2eaa9bd848e8235b688369b809128595a16d1b782a311626a0542855b94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setPosition = {
  startCell: 'startCell-value',
  endCell: 'endCell-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition')
    .post(setPosition);

```