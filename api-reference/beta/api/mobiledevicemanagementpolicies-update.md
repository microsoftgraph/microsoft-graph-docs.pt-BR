---
title: Atualizar mobileDeviceManagementPolicy
description: Atualize as propriedades de um objeto de gerenciamento de dispositivo móvel.
author: ravennMSFT
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6c0f0a40c7369b1ea7396c1a64af97bafc033f85
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023816"
---
# <a name="update-mobiledevicemanagementpolicy"></a>Atualizar mobileDeviceManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.Read.All, Policy.ReadWrite.MobilityManagement|
|Delegado (conta pessoal da Microsoft) | Sem suporte.|
|Aplicativo | Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)

No corpo da solicitação, fornece os valores para os campos listados abaixo que devem ser atualizados. **Observação:** Não é possível `PATCH` usar a operação com as outras `appliesTo` propriedades.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appliesTo|policyScope|Determina os grupos aos quais essa configuração de política se aplica. Os valores possíveis são: `none` , `all` , `selected` **Importante:** `selected` não pode ser usado ao especificar essa propriedade. Use [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) para adicionar grupos específicos. O `all` uso removerá todos os grupos existentes.|
|complianceUrl|Cadeia de caracteres|URL de conformidade do aplicativo de gerenciamento de mobilidade|
|discoveryUrl|Cadeia de caracteres|URL de descoberta do aplicativo de gerenciamento de mobilidade|
|termsOfUseUrl|String|TERMOS DE USO URL do aplicativo de gerenciamento de mobilidade|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.uem.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.uem.contoso.com/TermsofUse.aspx"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-mobilitymanagementpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
