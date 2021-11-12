---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d5438f0c62a43121a650a1df28c6bb3048b349abb825c492e48d193f275d1ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartLineFormat = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line')
    .version('beta')
    .get();

```