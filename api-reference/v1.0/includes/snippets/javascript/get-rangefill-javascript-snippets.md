---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22dfe0ac72af84837f073e8d8b89b32a30e3c74815453cc4228508dc77ed8119
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFill = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .get();

```