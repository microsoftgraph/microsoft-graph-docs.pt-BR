---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6d42f7728533e132133e836fe92911eddaa770a
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11014/assignments/19002')
    .version('beta')
    .delete();

```