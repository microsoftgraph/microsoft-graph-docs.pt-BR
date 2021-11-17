---
title: 'managementAction: apply'
description: Aplica uma ação de gerenciamento a um locatário gerenciado específico. Ao executar essa operação, as configurações apropriadas serão feitas e as políticas serão criadas. Por exemplo, ao aplicar a autenticação multifacional necessária para a ação de gerenciamento de administradores, criará uma política de acesso condicional Azure Active Directory que requer autenticação multifacional para todos os usuários que foram atribuídos a uma função de diretório administrativo.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 25b60d217a312a28210106b62f609c07384de904
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980940"
---
# <a name="managementaction-apply"></a>managementAction: apply
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aplica uma ação de gerenciamento a um locatário gerenciado específico. Ao executar essa operação, as configurações apropriadas serão feitas e as políticas serão criadas. Por exemplo, ao aplicar a autenticação multifacional necessária para a ação de gerenciamento de administradores, criará uma política de acesso condicional Azure Active Directory que requer autenticação multifacional para todos os usuários que foram atribuídos a uma função de diretório administrativo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ManagedTenants.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)|
|tenantGroupId|Cadeia de caracteres|O identificador do grupo de locatários.|
|managementTemplateId|String|O identificador do modelo [de gerenciamento](../resources/managedtenants-managementtemplate.md).|

## <a name="response"></a>Resposta

Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managementaction_apply"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
Content-Type: application/json

{
  "tenantId": "String",
  "tenantGroupId": "String",
  "managementTemplateId": "String"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementaction-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementaction-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementaction-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementaction-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/managementaction-apply-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.managedTenants.ManagementActionDeploymentStatus",
  "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
  "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9",
  "status": "completed",
  "workloadActionDeploymentStatuses": [
    {
      "actionId": "46b80b42-06c7-45b4-b6fb-aa0aecace87b",
      "status": "completed",
      "deployedPolicyId": null,
      "lastDeploymentDateTime": "2021-07-11T19:35:10.4463799Z",
      "error": null
    }
  ]
}
```
