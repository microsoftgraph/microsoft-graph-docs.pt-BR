---
title: Atualizar retentionEventType
description: Atualize as propriedades de um objeto retentionEventType.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 8710185656b1d9a9db7cdb1bbe631fa6049d0195
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447481"
---
# <a name="update-retentioneventtype"></a>Atualizar retentionEventType
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto retentionEventType](../resources/security-retentioneventtype.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|RecordsManagement.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/labels/retentionLabels/{retentionLabelId}/eventType
PATCH /security/triggerTypes/retentionEventTypes/{retentionEventTypeId}
PATCH /security/triggers/retentionEvents/{retentionEventId}/retentionEventType
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome do tipo de evento. Opcional.|
|descrição|Cadeia de caracteres|Informações sobre o tipo de evento. Opcional.|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|O usuário que criou o retentionEventType. Opcional.|
|createdDateTime|DateTimeOffset|A data em que o retentionEventType foi criado. Opcional.|
|lastModifiedBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|O usuário que modificou o retentionEventType pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data mais recente em que o retentionEventType foi modificado. Opcional.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_retentioneventtype"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/labels/retentionLabels/{retentionLabelId}/eventType
Content-Type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.security.retentionEventType",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
   "@odata.type": "microsoft.graph.security.retentionEventType"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.retentionEventType",
  "id": "dd689e79-9e79-dd68-799e-68dd799e68dd",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```
