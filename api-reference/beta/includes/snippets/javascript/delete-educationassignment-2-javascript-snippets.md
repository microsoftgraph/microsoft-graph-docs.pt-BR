---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d033014de398af8b887b27c3d4cb6b14b21fc1702de7e4744b0d42c258649fef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214119"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11014/assignmentCategories/19002')
    .version('beta')
    .delete();

```