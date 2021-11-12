---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 959b360e67a2a5cce2c55a1bd9282f7ea0503e4b045f4ac573efb57e0d02d711
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)')
    .version('beta')
    .get();

```