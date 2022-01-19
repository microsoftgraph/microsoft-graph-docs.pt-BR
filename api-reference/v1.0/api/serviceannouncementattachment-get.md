---
title: Obter serviceAnnouncementAttachment
description: Leia as propriedades e as relações de um objeto serviceAnnouncementAttachment.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: b589dc90d23c3aea9c5d23f42db2fa83f43760d9
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072734"
---
# <a name="get-serviceannouncementattachment"></a>Obter serviceAnnouncementAttachment
Namespace: microsoft.graph

Leia as propriedades e as relações de um [objeto serviceAnnouncementAttachment.](../resources/serviceannouncementattachment.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ServiceMessage.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|ServiceMessage.Read.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages/{serviceUpdateMessageId}/attachments/{serviceAnnouncementAttachmentId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-an-attachment-message-id"></a>Exemplo 1: Obter uma ID de mensagem de anexo

A solicitação a seguir retorna [um recurso serviceAnnouncementAttachment.](../resources/serviceannouncementattachment.md)

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_serviceannouncementattachment"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/admin/serviceAnnouncement/messages/MC54091/attachments/30356a46-ffad-47e1-acf6-40a99b1538c1
```

#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceAnnouncementAttachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft-ppe.com/v1.0/$metadata#admin/serviceAnnouncement/messages('MC54091')/attachments/$entity",
    "contentType": "application/csv",
    "isInline": false,
    "lastModifiedDateTime": "2021-09-21T04:07:15.9720778Z",
    "name": "An attachment for a Data Privacy message regarding your organization is available within Message Center. The contents of this attachment can be accessed within Message Center by a Global Administrator or someone designated as a Message Center Privacy Reader. Please sign in to Admin Center to view the details of this message in the Microsoft 365 Message center.",
    "size": 44583,
    "id": "30356a46-ffad-47e1-acf6-40a99b1538c1"
  }
}
```

### <a name="example-2-return-a-file-stream-of-an-attachment-content-for-a-message"></a>Exemplo 2: Retornar um fluxo de arquivo de um conteúdo de anexo para uma mensagem

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_serviceannouncementattachment"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/admin/serviceAnnouncement/messages/MC54091/attachments/30356a46-ffad-47e1-acf6-40a99b1538c1/content
```

#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceAnnouncementAttachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": "An attachment for a Data Privacy message regarding your organization is available within Message Center. The contents of this attachment can be accessed within Message Center by a Global Administrator or someone designated as a Message Center Privacy Reader. Please sign in to Admin Center to view the details of this message in the Microsoft 365 Message center."
}
```
