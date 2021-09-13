---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66c8392b078b134322ffb99b0aa98ef3b6e9bc25
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59090207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/{id}/participants/{id}')
    .version('beta')
    .delete();

```