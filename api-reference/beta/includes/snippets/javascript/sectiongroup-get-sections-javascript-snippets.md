---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ce3aafce158c5ebe0bc1f264347f1d140c5901d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .version('beta')
    .get();

```