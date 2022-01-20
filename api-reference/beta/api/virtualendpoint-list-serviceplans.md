---
title: Listar servicePlans
description: Listar os planos de serviço disponíveis no momento que uma organização pode comprar para seus PCs de Nuvem.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6490cc8fc920894e789caf17776a34c3bb105839
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092706"
---
# <a name="list-serviceplans"></a>Listar servicePlans

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar os planos de serviço disponíveis no momento que uma organização pode comprar para seus PCs de Nuvem.

Para exemplos de planos de serviço disponíveis no momento, consulte [Windows 365 comparar planos e preços.](https://www.microsoft.com/windows-365/business/compare-plans-pricing) Atualmente, a API Graph microsoft está disponível para Windows 365 Enterprise.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CloudPC.Read.All, CloudPC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/servicePlans
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [cloudPcServicePlan](../resources/cloudpcserviceplan.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_servicePlans"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/servicePlans
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceplans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-serviceplans-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-serviceplans-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcServicePlan",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcServicePlan",
      "id": "dea1edd3-edd3-dea1-d3ed-a1ded3eda1de",
      "displayName": "Cloud PC - Level 1 - 1vCPU/2GB",
      "type": "enterprise",
      "vCpuCount": 1,
      "ramInGB": 2,
      "storageInGB": 64,
      "userProfileInGB": 25
    }
  ]
}
```
