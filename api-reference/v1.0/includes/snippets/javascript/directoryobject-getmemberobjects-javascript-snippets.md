---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00a19721ce25e88603d616941dddfca6c5fdeadb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809274"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/directoryObjects/{object-id}/getMemberObjects')
    .post(string);

```