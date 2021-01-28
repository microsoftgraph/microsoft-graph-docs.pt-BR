---
title: Atualizar educationAssignmentSettings
description: Atualizar as propriedades de um objeto educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0475f49b400b12e8716fcb2ba122c99cf46f4b1e
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034321"
---
# <a name="update-educationassignmentsettings"></a>Atualizar educationAssignmentSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar as propriedades de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md) Somente professores podem atualizar essas configurações.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/{id}/assignmentSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) .

A tabela a seguir mostra as propriedades que são necessárias ao atualizar [educationAssignmentSettings](../resources/educationassignmentsettings.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|submissionAnimationDisabled|Boolean|Indica se a animação de celebração de turn-in será mostrada. Um valor indica `true` que a animação não será mostrada. O valor padrão é `false`.|



## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "submissionAnimationDisabled": true
}
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "submissionAnimationDisabled": true
}
```

