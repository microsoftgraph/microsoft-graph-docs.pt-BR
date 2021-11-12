---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af3d96e71d117b90c3b3f815e9cb9b0e206dca8ab0da43556b858e1c65974921
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216365"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookFormatProtection = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/protection')
    .version('beta')
    .get();

```