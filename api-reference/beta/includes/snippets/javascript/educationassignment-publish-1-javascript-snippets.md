---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 697aac5422c3ec060afced0a6e80622e68c647ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/education/classes/11012/assignments/19002/getResourcesFolderUrl')
    .version('beta')
    .get();

```