---
title: Tipo de recurso deviceManagementResourceAccessProfileBase
description: Tipo de perfil base para acesso a recursos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d795d99e2d3808268100c22ac8d9840edd96c85
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151813"
---
# <a name="devicemanagementresourceaccessprofilebase-resource-type"></a>Tipo de recurso deviceManagementResourceAccessProfileBase

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de perfil base para acesso a recursos

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementResourceAccessProfileBases](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-list.md)|[Coleção deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Listar propriedades e relações dos [objetos deviceManagementResourceAccessProfileBase.](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|[Obter deviceManagementResourceAccessProfileBase](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-get.md)|[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|Leia propriedades e relações do [objeto deviceManagementResourceAccessProfileBase.](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|[atribuir ação](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-assign.md)|[Coleção deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|Ainda não documentado|
|[ação queryByPlatformType](../api/intune-rapolicy-devicemanagementresourceaccessprofilebase-querybyplatformtype.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador de perfil|
|versão|Int32|Versão do perfil|
|displayName|Cadeia de caracteres|Nome de exibição de perfil|
|descrição|Cadeia de caracteres|Descrição do perfil|
|creationDateTime|DateTimeOffset|O perfil DateTime foi criado|
|lastModifiedDateTime|DateTimeOffset|O perfil DateTime foi modificado pela última vez|
|roleScopeTagIds|Coleção de cadeias de caracteres|Marcas de escopo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo.|

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




