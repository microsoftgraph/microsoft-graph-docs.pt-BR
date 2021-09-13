---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19705536a2685f26663fb8eb84c3d1da2875166127ebc8e6fa61c12a0e224ef9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: 'Sheet1!A1:D5',
  hasHeaders: true
};

await client.api('/me/drive/items/{id}/workbook/tables/add')
    .post(workbookTable);

```