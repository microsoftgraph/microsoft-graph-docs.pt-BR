---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2aba128e4c781dab30f226e25f5240e1f95db17
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38078333"
---
# <a name="auditactor-resource-type"></a>Tipo de recurso auditActor

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades para Ator de auditoria.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|String|Tipo de ator.|
|userPermissions|Conjunto de cadeia de caracteres|Lista de permissões de usuário de quando a auditoria foi executada.|
|ApplicationId|String|ID do aplicativo AAD.|
|applicationDisplayName|String|Nome do aplicativo.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário (UPN).|
|servicePrincipalName|String|Nome da entidade de serviço (SPN).|
|ipAddress|String|IPAddress.|
|userId|Cadeia de caracteres|ID do usuário.|
|userRoleScopeTags|coleção [roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)|Lista de marcas de escopo de usuário quando a auditoria foi realizada.|

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
  ]
}
```



