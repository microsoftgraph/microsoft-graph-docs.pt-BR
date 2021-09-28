---
title: 'reportRoot: getAttackSimulationRepeatOffenders'
description: Listar usuários infratores repetidos de um locatário em campanhas de treinamento e simulação de ataques.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 176cb052190c20ec5e99d1e3f6d19d4ec743c162
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979459"
---
# <a name="reportroot-getattacksimulationrepeatoffenders"></a>reportRoot: getAttackSimulationRepeatOffenders
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar os usuários de um locatário que tenha rendido a ataques mais de uma vez em campanhas de treinamento e simulação de ataques.

Esta função é `@odata.nextLink` compatível com paginação.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                            |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Reports.Read.All                            |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getAttackSimulationRepeatOffenders
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção attackSimulationRepeatOffender](../resources/attacksimulationrepeatoffender.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "reportroot_getattacksimulationrepeatoffenders"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAttackSimulationRepeatOffenders
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attackSimulationRepeatOffender)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "repeatOffenceCount": 1,
      "attackSimulationUser": {
        "userId": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      }
    }
  ]
}
```

