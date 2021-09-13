---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d68b38f1735e4d099389e6f74b37a1c4431bf6195609b71c58d6c5ce1eb91fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406710"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workingHours = await client.api('/me/mailboxSettings/workingHours')
    .get();

```