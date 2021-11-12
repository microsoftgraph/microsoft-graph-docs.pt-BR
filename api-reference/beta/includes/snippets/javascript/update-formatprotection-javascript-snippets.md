---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9145640be3ec7104e5111f8d23420fd410ba5975e621e6baae1681c14748b7c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookFormatProtection = {
  locked: true,
  formulaHidden: true
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/protection')
    .version('beta')
    .update(workbookFormatProtection);

```