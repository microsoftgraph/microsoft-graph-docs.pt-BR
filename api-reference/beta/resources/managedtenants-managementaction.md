---
title: Tipo de recurso managementAction
description: Representa uma ação de gerenciamento de linha de base para um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 156d4ff0d7ffb9574793ccdd5d56bc2a89cd3b22
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402144"
---
# <a name="managementaction-resource-type"></a>Tipo de recurso managementAction

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma ação de gerenciamento de linha de base para um determinado locatário gerenciado. Exemplos de ações de gerenciamento são criptografia de dispositivo, configurações para permitir Azure Active Directory registro de dispositivos e exigir autenticação multifa factor para administradores.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Gerenciamento de listasActions](../api/managedtenants-managedtenant-list-managementactions.md)|[Coleção microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|Obter uma lista dos [objetos managementAction](../resources/managedtenants-managementaction.md) e suas propriedades.|
|[Obter managementAction](../api/managedtenants-managementaction-get.md)|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|Leia as propriedades e as relações de um [objeto managementAction.](../resources/managedtenants-managementaction.md)|
|[apply](../api/managedtenants-managementaction-apply.md)|[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md)|Aplica as ações de gerenciamento ao locatário gerenciado.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Ferramentas para desenvolvedores|managementCategory|A categoria da ação de gerenciamento. Os valores possíveis são: `custom`, `devices`, `identity`, `unknownFutureValue`. Opcional. Somente leitura.|
|description|Cadeia de caracteres|A descrição da ação de gerenciamento. Opcional. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição da ação de gerenciamento. Opcional. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo da ação de gerenciamento. Obrigatório. Somente leitura.|
|referenceTemplateId|Cadeia de caracteres|A referência para o modelo de gerenciamento usado para gerar a ação de gerenciamento. Obrigatório. Somente leitura.|
|workloadActions|[coleção microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)|O conjunto de ações de carga de trabalho associadas à ação de gerenciamento. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementAction",
  "id": "String (identifier)",
  "referenceTemplateId": "String",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
