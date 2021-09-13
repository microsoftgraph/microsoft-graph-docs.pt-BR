---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce1680710875584c12ad7864a9967f7e2ba112b6ef51749bae67f62a04f12f7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clone = {
     displayName: 'Library Assist',
     description: 'Self help community for library',
     mailNickname: 'libassist',
     partsToClone: 'apps,tabs,settings,channels,members',
     visibility: 'public'
};

await client.api('/teams/{id}/clone')
    .post(clone);

```