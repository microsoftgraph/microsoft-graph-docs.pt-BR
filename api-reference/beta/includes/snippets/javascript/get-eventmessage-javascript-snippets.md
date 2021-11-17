---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8cde4e6ddc16d2fb50303402d5459004d232f91a4e88cdf02ffdc1502b95d81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkADYAAAImV_lAAA=')
    .version('beta')
    .get();

```