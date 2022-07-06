---
title: Criar taskFileAttachment
description: Adicione um novo objeto taskFileAttachment a um todoTask.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 590e8912178cdbc6eb0c2ed9f756ff2a77e84f9e
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645598"
---
# <a name="create-taskfileattachment"></a>Criar taskFileAttachment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione um novo [objeto taskFileAttachment](../resources/taskfileattachment.md) a um [todoTask](../resources/todotask.md).

Essa operação limita o tamanho do anexo ao qual você pode adicionar menos de 3 MB. Se o tamanho dos anexos de arquivo for maior que 3 MB, [crie uma sessão de upload](../api/taskfileattachment-createuploadsession.md) para carregar os anexos.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Tasks.ReadWrite|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{id}/tasks/{id}/attachments
POST /users/{id}/todo/lists/{id}/tasks/{id}/attachments
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto taskFileAttachment](../resources/taskfileattachment.md) .

Ao criar um anexo de arquivo, inclua `"@odata.type": "#microsoft.graph.taskFileAttachment"` e as propriedades necessárias.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentBytes|Binária|O conteúdo do arquivo codificado pela base64. Obrigatório.|
|contentType|String|O tipo de conteúdo do anexo. |
|nome|Cadeia de caracteres|O nome do texto exibido sob o ícone que representa o anexo inserido. Não precisa ser o nome real do arquivo. Obrigatório. |
|size|Int32|O tamanho do anexo em bytes. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto taskFileAttachment](../resources/taskfileattachment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_taskFileAttachment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AAMkpsDRVK=/tasks/AAKdfjhgsjhgJ=/attachments
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "name": "smile",
  "contentBytes": "a0b1c76de9f7=",
  "contentType": "image/gif"
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taskFileAttachment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "id": "AAMkADNkN2R",
  "lastModifiedDateTime": "2017-01-26T08:48:28Z",
  "name": "smile",
  "contentType": "image/gif",
  "size": 1008
}
```

