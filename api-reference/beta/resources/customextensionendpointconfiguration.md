---
title: Tipo de recurso customExtensionEndpointConfiguration
description: Tipo de base abstrata que expõe os tipos derivados usados para configurar a propriedade endpointConfiguration de um objeto de extensão de fluxo de trabalho de pacote de acesso personalizado.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8607ee8311c0cfc64eef06c3dc2716fb775473fa
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338140"
---
# <a name="customextensionendpointconfiguration-resource-type"></a>Tipo de recurso customExtensionEndpointConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo de base abstrata que expõe os tipos derivados usados para configurar a propriedade **endpointConfiguration** de um [objeto](customaccesspackageworkflowextension.md) de extensão de fluxo de trabalho de pacote de acesso personalizado. Esse tipo abstrato é herdado pelo [objeto logicAppTriggerEndpointConfiguration](logicapptriggerendpointconfiguration.md) .

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration",
  "abstract": true
}
-->
``` json
{ 
  "@odata.type": "#microsoft.graph.customExtensionEndpointConfiguration" 
} 
```