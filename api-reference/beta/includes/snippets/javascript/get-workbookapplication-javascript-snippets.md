---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecd57ce7e2d27da8bfda3c521a27754d47213073e44970cfd825bd0cf1cc4afc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376072"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookApplication = await client.api('/me/drive/items/{id}/workbook/application')
    .version('beta')
    .get();

```