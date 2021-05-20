---
title: Atualizar mobileAppManagementPolicy
description: Atualize as propriedades de um objeto de política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 49c181f688fae97e0c9f58ecf68d830f3ca042fa
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547311"
---
# <a name="update-mobileappmanagementpolicy"></a>Atualizar mobileAppManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.Read.All, Policy.ReadWrite.All|
|Delegado (conta pessoal da Microsoft) | Sem suporte.|
|Aplicativo | Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileAppManagementPolicies/{id}
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
|appliesTo|policyScope|Determina os grupos aos quais essa configuração de política se aplica. Os valores possíveis são: `none` , `all` , `selected` **Importante:** `selected` não pode ser usado ao especificar essa propriedade. Use [includedGroups](../api/mobileappmanagementpolicies-post-includedgroups.md) para adicionar grupos específicos.|
|complianceUrl|String|URL de conformidade do aplicativo de gerenciamento de mobilidade|
|discoveryUrl|String|URL de descoberta do aplicativo de gerenciamento de mobilidade|
|termsOfUseUrl|String|TERMOS DE USO URL do aplicativo de gerenciamento de mobilidade|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.mg.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.mg.contoso.com/TermsofUse.aspx"
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
