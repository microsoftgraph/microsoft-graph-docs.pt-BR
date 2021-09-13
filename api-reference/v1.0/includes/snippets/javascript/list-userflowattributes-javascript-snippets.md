---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2df0aff0f7848eefe4bb1ae0f4b73f38f15c37f73e0764da57a0a0d49980233
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowAttributes = await client.api('/identity/userFlowAttributes')
    .get();

```