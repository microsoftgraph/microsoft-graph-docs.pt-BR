---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 186d6cacb4835578f216a641085ad32af34260014261266f75fadce5ebd0c466
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/groups/{id}/members')
    .get();

```