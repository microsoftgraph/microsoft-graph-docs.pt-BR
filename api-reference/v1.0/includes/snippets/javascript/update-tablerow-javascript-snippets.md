---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9037395278b588dd7406172fce55069307b6f14d6dc17517af47b694388a3925
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407009"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 99,
  values: 'values-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .update(workbookTableRow);

```