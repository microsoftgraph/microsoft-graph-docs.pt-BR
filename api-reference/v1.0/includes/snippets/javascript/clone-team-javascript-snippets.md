---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 510707a04e9b3d291ec15c275cc6b05f6af9049a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clone = {
     displayName: "Library Assist",
     description: "Self help community for library",
     mailNickname: "libassist",
     partsToClone: "apps,tabs,settings,channels,members",
     visibility: "public"
};

let res = await client.api('/teams/{id}/clone')
    .post(clone);

```