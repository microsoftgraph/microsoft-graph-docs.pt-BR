---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 035c60ae09b659e1691f43f1e1563dce51a04020
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882815"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)')
    .get();

```