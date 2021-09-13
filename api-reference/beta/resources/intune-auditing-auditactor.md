---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 258624d97663da9b25ee6552e7eb3430191c135b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146797"
---
# <a name="auditactor-resource-type"></a>Tipo de recurso auditActor

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades para Ator de auditoria.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tipo|Cadeia de caracteres|Tipo de ator.|
|userPermissions|Conjunto de cadeia de caracteres|Lista de permissões de usuário de quando a auditoria foi executada.|
|ApplicationId|Cadeia de caracteres|ID do aplicativo AAD.|
|applicationDisplayName|Cadeia de caracteres|Nome do aplicativo.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário (UPN).|
|servicePrincipalName|Cadeia de caracteres|Nome da entidade de serviço (SPN).|
|ipAddress|Cadeia de caracteres|IPAddress.|
|userId|Cadeia de caracteres|ID do usuário.|
|userRoleScopeTags|[Coleção roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)|Lista de marcas de escopo do usuário quando a auditoria foi realizada.|
|remoteTenantId|Cadeia de Caracteres|ID de locatário remoto|
|remoteUserId|Cadeia de Caracteres|ID do usuário remoto|

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



