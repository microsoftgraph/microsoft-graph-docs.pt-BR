---
title: 'aprovação: filterByCurrentUser'
description: Obter os recursos de aprovação da propriedade de navegação accessPackageAssignmentApprovals para o usuário atual.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7087edc3e9a69abc1f31cdf32f9d182903327d25
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63398071"
---
# <a name="approval-filterbycurrentuser"></a>aprovação: filterByCurrentUser
Namespace: microsoft.graph

No gerenciamento de direitos do Azure AD, retorne uma coleção de aprovações de atribuição [de pacote de acesso](../resources/approval.md). Os objetos retornados são aqueles que o usuário de chamada está no escopo de ser um aprovador.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/filterByCurrentUser(on='approver')
```

## <a name="function-parameters"></a>Parâmetros de função
Este método dá suporte aos parâmetros de consulta OData para pajamento por meio de um conjunto de resultados grande. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|on|approvalFilterByCurrentUserOptions| O valor permitido é `approver`. Obrigatório.|

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [de](../resources/approval.md) aprovação no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "approvalthis-filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/filterByCurrentUser(on='approver')
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.approval)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.approval",
      "id": "368f6786-6786-368f-8667-8f3686678f36"
    }
  ]
}
```

