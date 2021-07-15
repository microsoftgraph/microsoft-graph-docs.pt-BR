---
title: 'managementActionTenantDeploymentStatus: changeDeploymentStatus'
description: Altera o status de implantação de nível de locatário para a ação de gerenciamento. Essas informações são usadas para fornecer informações sobre quais ações de gerenciamento estão em um estado específico. Como exemplo, pode haver um plano para aplicar a autenticação multifator necessária para administradores, portanto, seria ideal alterar o status para planejado para refletir o status apropriado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 572ee7f6c6769ec500c47edee5d35dd18fe75d3f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440901"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a>managementActionTenantDeploymentStatus: changeDeploymentStatus
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Altera o status de implantação de nível de locatário para a ação de gerenciamento. Essas informações são usadas para fornecer informações sobre quais ações de gerenciamento estão em um estado específico. Como exemplo, pode haver um plano para aplicar a autenticação multifator necessária para administradores, portanto, seria ideal alterar o status para planejado para refletir o status apropriado.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ManagedTenants.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
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
|tenantGroupId|Cadeia de caracteres|O identificador do grupo de locatários.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)|
|managementActionId|Cadeia de caracteres|O identificador da ação [de gerenciamento](../resources/managedtenants-managementaction.md).|
|managementTemplateId|Cadeia de caracteres|O identificador do modelo [de gerenciamento](../resources/managedtenants-managementtemplate.md).|
|status|Cadeia de caracteres|O novo status para a [implantação do](../resources/managedtenants-managementaction.md) locatário de ações de gerenciamento.|

## <a name="response"></a>Resposta

Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managementactiontenantdeploymentstatus_changedeploymentstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
Content-Type: application/json
Content-length: 153

{
  "tenantGroupId": "String",
  "tenantId": "String",
  "managementActionId": "String",
  "managementTemplateId": "String",
  "status": "String"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementactiontenantdeploymentstatus-changedeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementactiontenantdeploymentstatus-changedeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementactiontenantdeploymentstatus-changedeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementactiontenantdeploymentstatus-changedeploymentstatus-java-snippets.md)]
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
  "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
  "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
  "status": "planned",
  "workloadActionDeploymentStatuses": []
}
```
