---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3d298435f024c40658dffd494398972cc754d09
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/termStore/groups')
    .version('beta')
    .get();

```