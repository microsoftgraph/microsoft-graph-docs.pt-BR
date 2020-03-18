---
title: tipo de recurso roleScopeTag
description: Marca de escopo de função
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d76ca4d2493b3d644c5b73c6b0645109573d3293
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773186"
---
# <a name="rolescopetag-resource-type"></a>tipo de recurso roleScopeTag

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Marca de escopo de função

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Listar Propriedades e relações dos objetos [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Obter roleScopeTag](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Leia as propriedades e as relações do objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Criar roleScopeTag](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Criar um novo objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Excluir roleScopeTag](../api/intune-rbac-rolescopetag-delete.md)|Nenhum|Exclui [roleScopeTag](../resources/intune-rbac-rolescopetag.md).|
|[Atualizar roleScopeTag](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Atualiza as propriedades de um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[atribuir ação](../api/intune-rbac-rolescopetag-assign.md)|coleção [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Ainda não documentado|
|[ação getRoleScopeTagsById](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|
|[função hasCustomRoleScopeTag](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|Booliano|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. É somente leitura e gerada automaticamente.|
|displayName|Cadeia de caracteres|O nome de exibição ou amigável da marca de escopo da função.|
|description|String|Descrição da marca de escopo da função.|
|isBuiltIn|Booliano|Descrição da marca de escopo da função.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|A lista de atribuições para esta marca de escopo de função.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isBuiltIn": true
}
```



