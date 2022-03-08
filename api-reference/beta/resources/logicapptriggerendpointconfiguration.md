---
title: Tipo de recurso logicAppTriggerEndpointConfiguration
description: Os detalhes de configuração para o ponto de extremidade do aplicativo lógico associado a uma extensão de fluxo de trabalho de pacote de acesso personalizado.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e7f97d944d2dffa8103ca53e04fd455d515fd41e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338153"
---
# <a name="logicapptriggerendpointconfiguration-resource-type"></a>Tipo de recurso logicAppTriggerEndpointConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os detalhes de configuração para o ponto de extremidade do aplicativo lógico associado a uma extensão de fluxo de trabalho de pacote de acesso personalizado. Derivado do [tipo abstrato customExtensionEndpointConfiguration](customextensionendpointconfiguration.md) .

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---| 
|logicAppWorkflowName|String|O nome do aplicativo lógico.|
|resourceGroupName|Cadeia de caracteres|O nome do grupo de recursos do Azure para o aplicativo lógico.|
|subscriptionId|String|Identificador da assinatura do Azure para o aplicativo lógico.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.logicAppTriggerEndpointConfiguration",
  "baseType": "microsoft.graph.customExtensionEndpointConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.logicAppTriggerEndpointConfiguration",
  "subscriptionId": "String",
  "resourceGroupName": "String",
  "logicAppWorkflowName": "String"
}
```
