---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52890a78e666d6c7205ed0e9dc59d2159605dd4d86517ab0af8090e591cc81f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/me/todo/lists')
    .get();

```