---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74e44caded510de3f0c60c2fb38bb60ceddcc65a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/66825e03-7ef5-42da-9069-724602c31f6b/presence')
    .get();

```