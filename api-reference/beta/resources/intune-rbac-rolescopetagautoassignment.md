---
title: tipo de recurso roleScopeTagAutoAssignment
description: Contém as propriedades da atribuição automática de uma marca de escopo de função a um grupo a ser aplicado a dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df95dff1efb35e6f8ac7d20ec99c83f89222786b
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177286"
---
# <a name="rolescopetagautoassignment-resource-type"></a>tipo de recurso roleScopeTagAutoAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades da atribuição automática de uma marca de escopo de função a um grupo a ser aplicado a dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar roleScopeTagAutoAssignments](../api/intune-rbac-rolescopetagautoassignment-list.md)|coleção [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Listar Propriedades e relações dos objetos [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .|
|[Obter roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Leia as propriedades e as relações do objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .|
|[Criar roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-create.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Criar um novo objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .|
|[Excluir roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-delete.md)|Nenhum|Exclui [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).|
|[Atualizar roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Atualiza as propriedades de um objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



