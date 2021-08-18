---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 731327393671442287ca3f9b5acd863ff9bde3be37432cbc416fc0bb4619abc2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156523"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}')
    .version('beta')
    .delete();

```