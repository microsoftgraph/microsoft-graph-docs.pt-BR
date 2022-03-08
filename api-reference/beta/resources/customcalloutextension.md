---
title: Tipo de recurso customCalloutExtension
description: Um tipo abstrato que define a configuração para aplicativos lógicos que podem ser integrados ao gerenciamento de direitos do cliente usam casos para implementar fluxos de trabalho de governança mais amplos. Esse tipo abstrato é herdado pelo tipo de recurso customAccessPackageWorkflowExtension
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7a76c37663fb3d9c5a49c1c539d1238d7423ba4a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338155"
---
# <a name="customcalloutextension-resource-type"></a>Tipo de recurso customCalloutExtension

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo abstrato que define a configuração para aplicativos lógicos que podem ser integrados ao gerenciamento de direitos do cliente usam casos para implementar fluxos de trabalho de governança mais amplos. Esse tipo abstrato é herdado pelo [tipo de recurso customAccessPackageWorkflowExtension](customaccesspackageworkflowextension.md) .

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authenticationConfiguration|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|Configuração para proteger a chamada da API para o aplicativo lógico. Por exemplo, o fluxo de credenciais do cliente OAuth. |
|clientConfiguration|[customExtensionClientConfiguration](../resources/customextensionclientconfiguration.md)| Configurações de conexão HTTP que definem por quanto tempo o Azure AD pode esperar por uma conexão com um aplicativo lógico, quantas vezes você pode repetir uma conexão com tempo de espera e os cenários de exceção quando as recuperações são permitidas.|
|descrição|String|Descrição do objeto customCalloutExtension.|
|displayName|String|Nome para exibição do objeto customCalloutExtension.|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|O tipo e os detalhes para configurar o ponto de extremidade para chamar o fluxo de trabalho do aplicativo lógico.|
|id|Cadeia de caracteres|Identificador do objeto customCalloutExtension. Herdado da [entidade](../resources/entity.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customCalloutExtension",
  "openType": false,
  "abstract": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customCalloutExtension",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "endpointConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration"
  },
  "clientConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
  },
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration"
  }
}
```

