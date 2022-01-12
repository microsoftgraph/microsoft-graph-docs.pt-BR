---
title: Tipo de recurso managementAction
description: Representa uma ação de gerenciamento de linha de base para um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f45bcabe1ab488bc5c19e83d7d34e52b92742a43
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61832601"
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
|description|String|A descrição da ação de gerenciamento. Opcional. Somente leitura.|
|displayName|String|O nome de exibição da ação de gerenciamento. Opcional. Somente leitura.|
|id|String|O identificador exclusivo da ação de gerenciamento. Obrigatório. Somente leitura.|
|referenceTemplateId|String|A referência para o modelo de gerenciamento usado para gerar a ação de gerenciamento. Obrigatório. Somente leitura.|
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
