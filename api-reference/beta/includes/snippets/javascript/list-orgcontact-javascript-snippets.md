---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90831dfe9676b6f7fac26daa51e35fad3e24281cf43780c124081062fba370a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .version('beta')
    .get();

```