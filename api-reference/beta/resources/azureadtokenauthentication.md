---
title: Tipo de recurso azureAdTokenAuthentication
description: Define o aplicativo do Azure AD usado para autenticar com uma extensão de fluxo de trabalho de pacote de acesso personalizado.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e1161897cf09ae1ad25d312b8ba5ca2bdf31617
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338045"
---
# <a name="azureadtokenauthentication-resource-type"></a>Tipo de recurso azureAdTokenAuthentication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o aplicativo do Azure AD usado para autenticar um aplicativo lógico com uma [extensão de](customaccesspackageworkflowextension.md) fluxo de trabalho de pacote de acesso personalizado. Somente a ID do aplicativo é necessária. Derivado de [customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|resourceId|Cadeia de caracteres|O **appID** do aplicativo do Azure AD a ser usado para autenticar um aplicativo lógico com uma extensão de fluxo de trabalho de pacote de acesso personalizado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureAdTokenAuthentication",
  "baseType": "microsoft.graph.customExtensionAuthenticationConfiguration"
}
-->

``` json
{ 
  "@odata.type": "#microsoft.graph.azureAdTokenAuthentication", 
  "resourceId": "String" 
 } 
```
