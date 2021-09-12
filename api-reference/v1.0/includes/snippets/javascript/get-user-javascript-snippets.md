---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa0d9c6060d9359a29cd85b85020f5e15983170364a042a9ac708ef5cc7217e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/me')
    .get();

```