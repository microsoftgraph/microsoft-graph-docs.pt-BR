---
title: Criar retentionLabel
description: Crie um novo objeto retentionLabel.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 492058e0b8ce292f8789a7f3e91ed36967f5f9a5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447483"
---
# <a name="create-retentionlabel"></a>Criar retentionLabel
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto retentionLabel](../resources/security-retentionlabel.md) .

Para criar um estágio [de revisão de](../resources/security-dispositionreviewstage.md) disposição, inclua a **propriedade actionAfterRetentionPeriod** no corpo da solicitação com um dos valores possíveis especificados.

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
POST /security/labels/retentionLabels
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto retentionLabel](../resources/security-retentionlabel.md) .

Especifique as propriedades a seguir ao criar **um retentionLabel**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionAfterRetentionPeriod|microsoft.graph.security.actionAfterRetentionPeriod| Especifica a ação a ser tomada em um documento com esse rótulo aplicado durante o período de retenção. Os valores possíveis são: `none`, `delete`, `startDispositionReview`, `unknownFutureValue`. |
|behaviorDuringRetentionPeriod|microsoft.graph.security.behaviorDuringRetentionPeriod|Especifica como o comportamento de um documento com esse rótulo deve ser durante o período de retenção. Os valores possíveis são: `doNotRetain`, `retain`, `retainAsRecord`, `retainAsRegulatoryRecord`, `unknownFutureValue`. |
|descriptionForAdmins|String|Fornece informações de rótulo para o administrador. Opcional. |
|descriptionForUsers|String|Fornece as informações de rótulo para o usuário. Opcional. |
|displayName|Cadeia de caracteres|Cadeia de caracteres exclusiva que define um nome de rótulo. |
|dispositionReviewStages|[coleção microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md)|Examine os estágios durante os quais os revisores são notificados para determinar se um documento deve ser excluído ou retido. |
|retentionDuration|[microsoft.graph.security.retentionDuration](../resources/security-retentionduration.md)|Especifica o número de dias para reter o conteúdo. |
|retentionTrigger|microsoft.graph.security.retentionTrigger|Especifica se a duração da retenção é calculada a partir da data de criação do conteúdo, da data rotulada ou da data da última modificação. Os valores possíveis são: `dateLabeled`, `dateCreated`, `dateModified`, `dateOfEvent`, `unknownFutureValue`. |
|defaultRecordBehavior|microsoft.graph.security.defaultRecordBehavior|Especifica o estado bloqueado ou desbloqueado de um rótulo de registro quando ele é criado. Os valores possíveis são: `startLocked`, `startUnlocked`, `unknownFutureValue`. |
|labelToBeApplied|Cadeia de caracteres|Especifica o rótulo de substituição a ser aplicado automaticamente após o término do período de retenção do rótulo atual. |



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_retentionlabel_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/labels/retentionLabels
Content-Type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.security.retentionLabel",
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
  "labelToBeApplied": "String",
  "defaultRecordBehavior": "String"
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.retentionLabel"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
```

