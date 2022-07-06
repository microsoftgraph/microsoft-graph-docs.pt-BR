---
title: 'taskFileAttachment: createUploadSession'
description: Crie uma sessão de upload para carregar iterativamente intervalos de um arquivo como um anexo para uma tarefa do Microsoft To Do.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a6a8aec00fcca1bbc50b25791c06db73cdd747f8
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645608"
---
# <a name="taskfileattachment-createuploadsession"></a>taskFileAttachment: createUploadSession
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma sessão de upload para carregar iterativamente intervalos de um arquivo como um anexo para um [todoTask](../resources/todotask.md).

Como parte da resposta, essa ação retorna uma URL de upload que você pode usar em `PUT` consultas sequenciais subsequentes. Os cabeçalhos de solicitação para cada `PUT` operação permitem que você especifique o intervalo exato de bytes a serem carregados. Isso permite que a transferência seja retomada, caso a conexão de rede seja descartada durante o upload.

A seguir estão as etapas para anexar um arquivo a uma tarefa do Microsoft To Do usando uma sessão de upload:

1. Crie uma sessão de upload.
2. Dentro dessa sessão de upload, carregue iterativamente intervalos de bytes (até 4 MB cada vez) até que todos os bytes do arquivo tenham sido carregados e o arquivo seja anexado ao **todoTask**.
3. Opcional: exclua a sessão de upload.

>**Nota:** Use essa abordagem para anexar um arquivo de qualquer tamanho com suporte entre 0 MB a 25 MB.

Para obter um exemplo que descreve o processo de anexo de ponta a ponta, consulte [anexar arquivos a uma tarefa Pendente](/graph/todo-attachments).

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
POST /me/todo/lists/{id}/tasks/{id}/attachments/createUploadSession
POST /users/{id}/todo/lists/{id}/tasks/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra o parâmetro que pode ser usado com essa ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|attachmentInfo|[attachmentInfo](../resources/attachmentinfo.md)|Representa atributos do item a ser carregado e anexado. No mínimo, especifique o tipo de anexo (`file`), um nome e o tamanho do arquivo.|


## <a name="response"></a>Resposta

Se tiver êxito, essa ação retornará `200 OK` um código de resposta e uma nova [uploadSession](../resources/uploadsession.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
A seguir está um exemplo de uma solicitação para criar uma sessão de upload.
<!-- {
  "blockType": "request",
  "name": "attachmentbasethis.createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachments/createUploadSession
Content-Type: application/json

{
  "attachmentInfo": {
    "@odata.type": "microsoft.graph.attachmentInfo",
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=",
    "expirationDateTime": "2022-06-09T10:45:27.4324526Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```