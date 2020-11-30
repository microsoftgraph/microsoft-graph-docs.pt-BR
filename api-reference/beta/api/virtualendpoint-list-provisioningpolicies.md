---
title: Listar cloudPcProvisioningPolicy
description: Exibir as propriedades e as relações de todas as políticas de provisionamento do Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b9d62152228518aa856b48e3fc064ce77fd1801f
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378249"
---
# <a name="list-provisioningpolicies"></a>Listar provisioningPolicies

Namespace: microsoft.graph

Listar Propriedades e relações dos objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC. ReadWrite. All, CloudPC. Read. All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece `$select` suporte `$filter` e `$expand` parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "list_cloudpcprovisioningpolicies"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcProvisioningPolicy)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
      "id": "1d164206-bf41-4fd2-8424-a3192d392273",
      "displayName": "Display Name value",
      "description": "Description value",
      "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
      "imageId": "Image ID value",
      "imageDisplayName": "Image Display Name value",
      "imageType":"custom"
    }
  ]
}
```
