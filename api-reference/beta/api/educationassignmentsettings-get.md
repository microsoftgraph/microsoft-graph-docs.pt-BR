---
title: Obter educationAssignmentSettings
description: Leia as propriedades e as relações de um objeto educationAssignmentSettings.
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bfd8a3377407ccdabfd2f9afece73fb2408e8945
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508769"
---
# <a name="get-educationassignmentsettings"></a>Obter educationAssignmentSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application| EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não fornece um corpo de solicitação para este método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignmentsettings
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "submissionAnimationDisabled": false
}
```

