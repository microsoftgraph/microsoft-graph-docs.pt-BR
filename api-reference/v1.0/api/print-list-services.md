---
title: Listar printServices
description: Recupere uma lista de objetos printService que representam os serviços disponíveis para seu locatário.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c5226eadd4edfd3e8d2d15534eed3fcb5ffc9619
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516882"
---
# <a name="list-printservices"></a>Listar printServices
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Recupere uma lista de **objetos printService** que representam os serviços disponíveis para seu locatário.

## <a name="permissions"></a>Permissões
Uma das permissões **de** Impressão Universal delegada [é](/graph/permissions-reference#universal-print-permissions) necessária para chamar essa API.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printService](../resources/printservice.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printService)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

