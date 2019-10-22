---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba3fe481771a2456bac05866560cee5317b0285c
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "35740993"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}')
    .delete();

```