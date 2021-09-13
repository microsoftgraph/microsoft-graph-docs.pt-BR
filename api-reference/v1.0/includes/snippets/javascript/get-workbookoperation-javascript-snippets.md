---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72bff4eb75fa2eb5dcf64158f7bd7c9aeda81c7e55546e5d36118c1c14d5cf38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookOperation = await client.api('/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}')
    .get();

```