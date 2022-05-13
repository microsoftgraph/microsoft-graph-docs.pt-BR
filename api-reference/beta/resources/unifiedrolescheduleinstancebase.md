---
title: Tipo de recurso unifiedRoleScheduleInstanceBase
description: Propriedade base da instância de agendamento de função unificada que combina a instância de agendamento de atribuição de função unificada e a instância de agendamento de qualificação de função unificada
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 78da74c6a867d6beed5dada2576d6248fc68ef37
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399443"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleInstanceBase

Namespace: microsoft.graph

Propriedade base da instância de agendamento de função unificada que combina instâncias de agendamento de atribuição de função unificada e instâncias de agendamento de qualificação de função unificada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. |
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. |
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleInstance. Chave, não anulável, somente leitura.|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança à qual a atribuição está sendo concedida. Pode ser um grupo ou um usuário. |
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se aplica. Somente leitura. <br> Suporta `$filter` (`eq`).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. |
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da atribuição. Habilita a recuperação do objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança que está obtendo uma atribuição de função por meio da solicitação. Habilita a recuperação da entidade de segurança `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|A roleDefinition para a atribuição. Habilita a recuperação da definição de `$expand` função usando ao mesmo tempo que obter a atribuição de função. O roleDefinition.Id é expandido automaticamente.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleInstanceBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String"
}
```
