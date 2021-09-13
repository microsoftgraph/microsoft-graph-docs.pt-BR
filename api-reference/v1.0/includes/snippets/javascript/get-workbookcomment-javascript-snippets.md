---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9f488a7dd2c5ea0270e9b7da5fa639b12e3498a9e94c2cfec4756afa007861c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100745"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookComment = await client.api('/drive/items/{id}/workbook/comments/{id}')
    .get();

```