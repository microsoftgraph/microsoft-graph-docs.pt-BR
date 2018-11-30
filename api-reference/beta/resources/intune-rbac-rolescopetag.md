---
title: tipo de recurso de roleScopeTag
description: Marca de escopo de função
ms.openlocfilehash: 9be1f1307243c18e10f8e6dfc3f302502cdb54a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036424"
---
# <a name="rolescopetag-resource-type"></a>tipo de recurso de roleScopeTag

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





