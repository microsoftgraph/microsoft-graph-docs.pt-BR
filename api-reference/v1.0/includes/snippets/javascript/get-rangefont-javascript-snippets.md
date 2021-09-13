---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0633486641d36b54998365acf8139847928a2403ca486a92dd6fa365d3db0706
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFont = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/font')
    .get();

```