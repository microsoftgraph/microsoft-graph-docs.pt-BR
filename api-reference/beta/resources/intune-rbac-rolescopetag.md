---
title: Tipo de recurso roleScopeTag
description: Marca de escopo de função
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d504565cbc5f37a70fc813386024b1c32c4654e6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063682"
---
# <a name="rolescopetag-resource-type"></a>Tipo de recurso roleScopeTag

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Marca de escopo de função

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|[Coleção roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Listar propriedades e relações dos [objetos roleScopeTag.](../resources/intune-rbac-rolescopetag.md)|
|[Obter roleScopeTag](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Leia propriedades e relações do [objeto roleScopeTag.](../resources/intune-rbac-rolescopetag.md)|
|[Criar roleScopeTag](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Crie um novo [objeto roleScopeTag.](../resources/intune-rbac-rolescopetag.md)|
|[Excluir roleScopeTag](../api/intune-rbac-rolescopetag-delete.md)|Nenhum|Exclui um [roleScopeTag](../resources/intune-rbac-rolescopetag.md).|
|[Atualizar roleScopeTag](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Atualize as propriedades de um [objeto roleScopeTag.](../resources/intune-rbac-rolescopetag.md)|
|[atribuir ação](../api/intune-rbac-rolescopetag-assign.md)|[Coleção roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Ainda não documentado|
|[Ação getRoleScopeTagsById](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|[Coleção roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Ainda não documentado|
|[função hasCustomRoleScopeTag](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|Booliano|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. É somente leitura e gerada automaticamente. Essa propriedade é somente leitura.|
|displayName|String|O nome de exibição ou amigável da Marca de Escopo de Função.|
|description|Cadeia de caracteres|Descrição da marca escopo de função.|
|isBuiltIn|Booliano|Descrição da marca escopo de função. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|A lista de atribuições para esta marca de escopo de função.|

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



