---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31b280c8e321088bcfb4cef419f4592774456c9a
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/comments/{id}/replies/{id}')
    .get();

```