---
title: Tipo de recurso cloudPcAuditActor
description: O ator de auditoria representado pelo usuário e aplicativo do Azure AD associado ao evento de auditoria.
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5cd851d22d20eb5d0e466cae7b799ad70bd390a2
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766310"
---
# <a name="cloudpcauditactor-resource-type"></a>Tipo de recurso cloudPcAuditActor

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O ator de auditoria representado pelo usuário e aplicativo do Azure AD associado ao evento de auditoria.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|[cloudPcAuditActorType](#cloudpcauditactortype-values)|O tipo de ator. Os valores possíveis `ItPro` `Application` incluem , e `Partner` `Unknown` .|
|userPermissions|Conjunto de cadeia de caracteres|Lista de permissões de usuário e permissões de aplicativo quando o evento de auditoria foi executado.|
|ApplicationId|Cadeia de caracteres|ID do aplicativo do Azure AD.|
|applicationDisplayName|Cadeia de caracteres|Nome do aplicativo.|
|userPrincipalName|String|Nome principal do usuário (UPN).|
|servicePrincipalName|Cadeia de caracteres|Nome da entidade de serviço (SPN).|
|ipAddress|Cadeia de caracteres|Endereço IP.|
|userId|Cadeia de caracteres|ID do usuário do Azure AD.|
|userRoleScopeTags|[Coleção cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md)|Lista de marcas de escopo de função.|
|remoteTenantId|Cadeia de caracteres|A ID do locatário do parceiro delegado.|
|remoteUserId|Cadeia de caracteres|A ID de usuário do parceiro delegada.|

### <a name="cloudpcauditactortype-values"></a>valores cloudPcAuditActorType

|Member|Descrição|
|:---|:---|
|itPro|A operação foi realizada por um profissional de IT.|
|aplicação|A operação foi executada pelo aplicativo.|
|partner|A operação foi realizada por um parceiro.|
|desconhecido|Ator desconhecido.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditActor"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```
