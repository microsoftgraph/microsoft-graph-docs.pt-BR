---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70782e0e922f05674171a3969a81ee38d02c1e6c61931b1e9fe1f0008086bd44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartAxis = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis')
    .get();

```