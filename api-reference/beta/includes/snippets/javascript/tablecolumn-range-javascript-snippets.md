---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65200ed2da04d710feb44611b46a313e21765e5164747e00847d69e29843f9dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/Range')
    .version('beta')
    .get();

```