---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b07088575fcb2e086e82c7234a1d87e90a3af73a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476176"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Stream = [
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
];

let res = await client.api('/me/onenote/pages/{id}/content')
    .update({Stream : Stream});

```