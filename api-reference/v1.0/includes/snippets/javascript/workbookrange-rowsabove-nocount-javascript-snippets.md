---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06e28f804bb2e43fc8b9b399cefe8805525d8dc0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsAbove')
    .get();

```