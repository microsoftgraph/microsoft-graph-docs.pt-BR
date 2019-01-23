---
title: tipo de recurso de roleScopeTag
description: Marca de escopo de função
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3a63ac05ea6161843aa1ad664a99003b7f69d38e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400561"
---
# <a name="rolescopetag-resource-type"></a>tipo de recurso de roleScopeTag

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Marca de escopo de função

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Lista as propriedades e os relacionamentos dos objetos [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Obter roleScopeTag](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Leia as propriedades e os relacionamentos do objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Criar roleScopeTag](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Crie um novo objeto de [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Excluir roleScopeTag](../api/intune-rbac-rolescopetag-delete.md)|Nenhum|Exclui um [roleScopeTag](../resources/intune-rbac-rolescopetag.md).|
|[Atualizar roleScopeTag](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Atualize as propriedades de um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. É somente leitura e é gerada automaticamente.|
|displayName|String|A exibição ou o nome amigável da marca de escopo de função.|
|description|String|Descrição da marca de escopo de função.|

## <a name="relationships"></a>Relações
Nenhum

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
  "description": "String"
}
```




