---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 903a4b74630e1542b8fca03ad16997f837882cec6a4d8dce349b12dac4192333
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extensionProperties = await client.api('/applications/{id}/extensionProperties')
    .get();

```