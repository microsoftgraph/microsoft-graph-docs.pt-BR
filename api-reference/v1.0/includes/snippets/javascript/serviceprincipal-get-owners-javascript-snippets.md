---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 667e80fd4d4e62b3f62064e4463ceef457eee8eb6b8a0b6365c060bea7c6e9ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/servicePrincipals/{id}/owners')
    .get();

```