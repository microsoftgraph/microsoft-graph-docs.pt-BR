---
title: Listar managedDeviceCompliances
description: Obter uma lista dos objetos managedDeviceCompliance e suas propriedades.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 869f37bcfc17d0321ba47894906a42c32922d62c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022115"
---
# <a name="list-manageddevicecompliances"></a>Listar managedDeviceCompliances
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [objetos managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-manageddevicecompliance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-manageddevicecompliance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-manageddevicecompliance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-manageddevicecompliance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-manageddevicecompliance-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managedDeviceCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#managedDeviceCompliances",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_6dd4fe4b-5ea2-4ab2-8ac4-7dd2995f1649",
      "managedDeviceId": "6dd4fe4b-5ea2-4ab2-8ac4-7dd2995f1649",
      "managedDeviceName": "VM2688",
      "complianceStatus": "Noncompliant",
      "osDescription": "Windows",
      "osVersion": "10.0.19042.1083",
      "lastSyncDateTime": "2021-07-09T14:38:56.379702Z",
      "ownerType": "Company",
      "model": "Virtual Machine",
      "manufacturer": "Microsoft Corporation",
      "inGracePeriodUntilDateTime": "2021-06-14T14:35:24.8225Z",
      "lastRefreshedDateTime": "2021-07-11T07:03:54.0326474Z",
      "deviceType": "WindowsRT",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_49ed91f1-32ac-4881-9c1b-b709ba29e31b",
      "managedDeviceId": "49ed91f1-32ac-4881-9c1b-b709ba29e31b",
      "managedDeviceName": "VM4511",
      "complianceStatus": "Noncompliant",
      "osDescription": "Windows",
      "osVersion": "10.0.19042.1052",
      "lastSyncDateTime": "2021-07-09T14:41:57.8785122Z",
      "ownerType": "Company",
      "model": "Virtual Machine",
      "manufacturer": "Microsoft Corporation",
      "inGracePeriodUntilDateTime": "2021-06-14T14:36:09.1851Z",
      "lastRefreshedDateTime": "2021-07-11T06:53:35.8484421Z",
      "deviceType": "WindowsRT",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
