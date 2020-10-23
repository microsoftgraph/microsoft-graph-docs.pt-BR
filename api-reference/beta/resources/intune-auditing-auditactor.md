---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05fdb86a13c7984975f9a3076909c06fcc5ecbe7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706076"
---
# <a name="auditactor-resource-type"></a>Tipo de recurso auditActor

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades para Ator de auditoria.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|String|Tipo de ator.|
|userPermissions|Conjunto de cadeia de caracteres|Lista de permissões de usuário de quando a auditoria foi executada.|
|ApplicationId|Cadeia de caracteres|ID do aplicativo AAD.|
|applicationDisplayName|Cadeia de caracteres|Nome do aplicativo.|
|userPrincipalName|String|Nome principal do usuário (UPN).|
|servicePrincipalName|Cadeia de caracteres|Nome da entidade de serviço (SPN).|
|ipAddress|Cadeia de caracteres|IPAddress.|
|userId|Cadeia de caracteres|ID do usuário.|
|userRoleScopeTags|coleção [roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)|Lista de marcas de escopo de usuário quando a auditoria foi realizada.|
|remoteTenantId|String|ID de locatário remoto|
|remoteUserId|String|ID de usuário remoto|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
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
      "@odata.type": "microsoft.graph.roleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```





