---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 290e505d7dc600681295aa5d92c7bbeb3ae8218b0b67e49bf687511a69779c0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear')
    .post();

```