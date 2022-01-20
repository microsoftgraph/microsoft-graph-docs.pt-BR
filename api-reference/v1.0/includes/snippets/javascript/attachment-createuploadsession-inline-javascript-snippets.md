---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac3be6cf38ccda2dbeb14761babb02b76d948dbc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const uploadSession = {
  AttachmentItem: {
    attachmentType: 'file',
    name: 'scenary', 
    size: 7208534,
    isInline: true,
    contentId: 'my_inline_picture'
  }
};

await client.api('/me/messages/AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA=/attachments/createUploadSession')
    .post(uploadSession);

```