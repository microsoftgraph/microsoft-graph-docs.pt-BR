---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f247a4df18a4a6d03ef65a7be15d92f3e7b2030229952b1ca6a3835257ad56aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/archive')
    .post();

```