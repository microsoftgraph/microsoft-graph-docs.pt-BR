---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 863f89a1086fc699b8a37fd2dbdc50494f396463bacb6d93e97c7ba47a6934ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let createdObjects = await client.api('/me/createdObjects')
    .get();

```