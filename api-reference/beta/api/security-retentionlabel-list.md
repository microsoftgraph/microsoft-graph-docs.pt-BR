---
title: Listar retentionLabels
description: Obtenha uma lista dos objetos retentionLabel e suas propriedades.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0981779968e9e4a7336333c48cddb2921431d5de
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439673"
---
# <a name="list-retentionlabels"></a>Listar retentionLabels
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos retentionLabel](../resources/security-retentionlabel.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|RecordsManagement.Read.All, RecordsManagement.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|RecordsManagement.Read.All, RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/labels/retentionLabels
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte à expansão dos parâmetros de consulta OData para ajudar a personalizar a resposta.  Por exemplo, para recuperar a **propriedade retentionEventType** , você pode usar o `expand` parâmetro:`$expand=retentionEventType`. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_retentionlabel"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/labels/retentionLabels
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.retentionLabel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.security.retentionLabel",
      "id": "64a99fb4-07be-0481-8746-44c15c0eef1f",
      "displayName": "String",
      "behaviorDuringRetentionPeriod": "String",
      "actionAfterRetentionPeriod": "String",
      "retentionTrigger": "String",
      "retentionDuration": {
        "@odata.type": "microsoft.graph.security.retentionDuration"
      },
      "isInUse": "Boolean",
      "descriptionForAdmins": "String",
      "descriptionForUsers": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "String (timestamp)",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "labelToBeApplied": "String",
      "defaultRecordBehavior": "String"
    }
  ]
}
```


