---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8323575cdda91770581601ebae2363f15d05d70713e0a1fdf04d7a49fa228f9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329881"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments')
    .get();

```