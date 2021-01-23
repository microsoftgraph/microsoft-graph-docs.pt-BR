---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c495c8ff816fe7d6253261d407aa3f4923add525
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/user')
    .version('beta')
    .get();

```