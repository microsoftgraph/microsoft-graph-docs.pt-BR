---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d12d7cf4f102fa370273edb6567e27dc9ec0f20a87af594738c63773e6b13936
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/LastColumn')
    .version('beta')
    .get();

```