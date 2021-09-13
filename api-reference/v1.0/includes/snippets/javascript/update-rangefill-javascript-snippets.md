---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53010f73e36ccef9c9cb5202f27f100fe64c315f97be100555b9b5938c87a829
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: 'color-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .update(workbookRangeFill);

```