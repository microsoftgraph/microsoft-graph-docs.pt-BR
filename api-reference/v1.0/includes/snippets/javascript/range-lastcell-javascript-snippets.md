---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5826790534fe254387a31ccf2ac2c216243fab94ed8c5ed6f2a87e402b124bf5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/lastCell')
    .get();

```