---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d38bee7a73867e232d916b93ae5f0062e89769025c26ba5575f93bc98076ce45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sites = await client.api('/sites/{site-id}/sites')
    .get();

```