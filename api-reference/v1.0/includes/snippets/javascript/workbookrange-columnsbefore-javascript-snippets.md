---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4afbcfeb447f4996b00dc1cedc9a9902f2ecb00c
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)')
    .get();

```