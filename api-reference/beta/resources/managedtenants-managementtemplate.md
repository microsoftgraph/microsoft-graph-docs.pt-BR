---
title: Tipo de recurso managementTemplate
description: Representa um grupo de ações e configurações que podem ser executadas em um locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 6dacd5d94c921ca4afd59219be24509f6879c5b8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792047"
---
# <a name="managementtemplate-resource-type"></a>Tipo de recurso managementTemplate

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo de ações e configurações que podem ser executadas em um locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Gerenciamento de listasTemplates](../api/managedtenants-managedtenant-list-managementtemplates.md)|[coleção microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Obter uma lista dos [objetos managementTemplate](../resources/managedtenants-managementtemplate.md) e suas propriedades.|
|[Obter managementTemplate](../api/managedtenants-managementtemplate-get.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Leia as propriedades e as relações de um [objeto managementTemplate.](../resources/managedtenants-managementtemplate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Ferramentas para desenvolvedores|managementCategory|A categoria de gerenciamento do modelo de gerenciamento. Os valores possíveis são: `custom`, `devices`, `identity`, `unknownFutureValue`. Obrigatório. Somente leitura.|
|description|String|A descrição do modelo de gerenciamento. Opcional. Somente leitura.|
|displayName|String|O nome de exibição do modelo de gerenciamento. Obrigatório. Somente leitura.|
|id|String|O identificador exclusivo do modelo de gerenciamento. Obrigatório. Somente leitura.|
|parameters|[coleção microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md)|A coleção de parâmetros usados pelo modelo de gerenciamento. Opcional. Somente leitura.|
|workloadActions|[coleção microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)|O conjunto de ações de carga de trabalho associadas ao modelo de gerenciamento. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.managedTenants.templateParameter"
    }
  ],
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
