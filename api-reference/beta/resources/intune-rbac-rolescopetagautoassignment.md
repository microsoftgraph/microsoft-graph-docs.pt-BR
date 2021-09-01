---
title: Tipo de recurso roleScopeTagAutoAssignment
description: Contém as propriedades para atribuir automaticamente uma Marca de Escopo de Função a um grupo a ser aplicado a Dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84bcaccc1206bb71e74e197bc7932a7a12ff6361
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806002"
---
# <a name="rolescopetagautoassignment-resource-type"></a>Tipo de recurso roleScopeTagAutoAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades para atribuir automaticamente uma Marca de Escopo de Função a um grupo a ser aplicado a Dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar roleScopeTagAutoAssignments](../api/intune-rbac-rolescopetagautoassignment-list.md)|[Coleção roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Listar propriedades e relações dos [objetos roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Obter roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Leia propriedades e relações do [objeto roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Criar roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-create.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Crie um novo [objeto roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|
|[Excluir roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-delete.md)|Nenhum(a)|Exclui um [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).|
|[Atualizar roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Atualize as propriedades de [um objeto roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Essa propriedade é somente leitura.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino da atribuição automática para a marca de escopo de função específica.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```



