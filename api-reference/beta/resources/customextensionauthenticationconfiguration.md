---
title: Tipo de recurso customExtensionAuthenticationConfiguration
description: Tipo de base abstrata que expõe a configuração da propriedade **authenticationConfiguration** dos tipos derivados que herdam do tipo abstrato customCalloutExtension
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3fbe85e5cca096ad0af24b7d0ffa04e035be63a9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337965"
---
# <a name="customextensionauthenticationconfiguration-resource-type"></a>Tipo de recurso customExtensionAuthenticationConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo de base abstrata que expõe a configuração da propriedade **authenticationConfiguration** dos tipos derivados que herdam do [tipo abstrato customCalloutExtension](customcalloutextension.md) . Esse tipo abstrato é herdado pelo tipo de recurso [azureAdTokenAuthentication](../resources/azureadtokenauthentication.md) .

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration",
  "abstract": true
}
-->

``` json
{ 
  "@odata.type": "#microsoft.graph.customExtensionAuthenticationConfiguration " 
} 
```