---
title: Listar anexos
description: Obter a lista de anexos associados a uma mensagem de serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 513692a2877d2e8589acb7d4f10bd5d09d88f7f5
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072782"
---
# <a name="list-attachments"></a>Listar anexos
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de anexos associados a uma mensagem de serviço.

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
GET /admin/serviceAnnouncement/messages/{serviceUpdateMessageId}/attachments
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-all-attachments-of-a-message-in-a-collection"></a>Exemplo 1: Obter todos os anexos de uma mensagem em uma coleção

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_serviceannouncementattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/MC54091/attachments
```

#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.serviceAnnouncementAttachment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context": "https://graph.microsoft-ppe.com/beta/$metadata#admin/serviceAnnouncement/messages('MC54091')/attachments",
    "value": [
        {
            "contentType": "application/csv",
            "isInline": false,
            "lastModifiedDateTime": "2021-09-21T04:07:15.9720778Z",
            "name": "An attachment for a Data Privacy message regarding your organization is available within Message Center. The contents of this attachment can be accessed within Message Center by a Global Administrator or someone designated as a Message Center Privacy Reader. Please sign in to Admin Center to view the details of this message in the Microsoft 365 Message center.",
            "size": 44583,
            "id": "30356a46-ffad-47e1-acf6-40a99b1538c1"
        },
        {
            "contentType": "application/csv",
            "isInline": false,
            "lastModifiedDateTime": "2021-09-21T04:07:15.9720778Z",
            "name": "An attachment for a Data Privacy message regarding your organization is available within Message Center. The contents of this attachment can be accessed within Message Center by a Global Administrator or someone designated as a Message Center Privacy Reader. Please sign in to Admin Center to view the details of this message in the Microsoft 365 Message center.",
            "size": 288849,
            "id": "fdd33417-37b9-49cc-95c1-7af90f2366c8"
        }
    ]
}
```

### <a name="example-2-get-a-zip-file-of-all-attachments-in-stream-for-a-message"></a>Exemplo 2: Obter um arquivo zip de todos os anexos no fluxo para uma mensagem

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_serviceannouncementattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/MC54091/attachmentsArchive
```

#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context": "https://graph.microsoft-ppe.com/beta/$metadata#admin/serviceAnnouncement/messages('MC54091')/attachmentsArchive",
    "value": "Stream"
}
```
