---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce3b2c6c3e107eea45accb385d9951beae8d8d14
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)')
    .version('beta')
    .get();

```