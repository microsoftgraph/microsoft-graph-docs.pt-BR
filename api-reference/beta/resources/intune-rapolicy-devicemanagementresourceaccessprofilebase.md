---
title: tipo de recurso deviceManagementResourceAccessProfileBase
description: Tipo de perfil básico para acesso de recurso
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df8389670d636d5ab556339ae4fc89217043663e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49336987"
---
# <a name="devicemanagementresourceaccessprofilebase-resource-type"></a>tipo de recurso deviceManagementResourceAccessProfileBase

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de perfil básico para acesso de recurso

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementResourceAccessProfileBases](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-list.md)|coleção [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Listar Propriedades e relações dos objetos [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) .|
|[Obter deviceManagementResourceAccessProfileBase](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-get.md)|[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Leia as propriedades e as relações do objeto [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md) .|
|[atribuir ação](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-assign.md)|coleção [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador de perfil|
|versão|Int32|Versão do perfil|
|displayName|String|Nome de exibição do perfil|
|description|String|Descrição do perfil|
|creationDatetime|DateTimeOffset|Perfil DateTime foi criado|
|lastModifiedDateTime|DateTimeOffset|Perfil DateTime modificado pela última vez|
|roleScopeTagIds|Coleção de cadeias de caracteres|Marcas de escopo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementResourceAccessProfileBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileBase",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




