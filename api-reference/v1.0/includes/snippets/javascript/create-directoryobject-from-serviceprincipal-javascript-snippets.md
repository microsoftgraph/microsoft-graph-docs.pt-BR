---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 542c4ba657e22657f7be58d1942eb4fbc93259d738126357ebea2b987a1cfa36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/servicePrincipals/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```