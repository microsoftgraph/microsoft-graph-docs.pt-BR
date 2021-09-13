---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 385bfcda8b947dae70b8861bd934fde0483119868b93c996e108b8aa2c0a2326
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange')
    .get();

```