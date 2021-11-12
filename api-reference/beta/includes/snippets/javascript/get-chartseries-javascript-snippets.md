---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0c76375c23539f2d7f5f4eecc0e82ad067de872bcc4331b370aae2a97a0f913
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartSeries = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}')
    .version('beta')
    .get();

```