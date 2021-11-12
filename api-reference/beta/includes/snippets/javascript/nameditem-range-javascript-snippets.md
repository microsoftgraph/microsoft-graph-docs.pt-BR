---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec094300bd1caad33e38a4f369c27c3196af030a7bfd35e087a80e533a0dfc84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/Range')
    .version('beta')
    .get();

```