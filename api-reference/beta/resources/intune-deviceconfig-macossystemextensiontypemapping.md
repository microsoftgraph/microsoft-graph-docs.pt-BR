---
title: Tipo de recurso macOSSystemExtensionTypeMapping
description: Representa um mapeamento entre identificadores de equipe para extensões do sistema macOS e tipos de extensão do sistema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4ae89a8d47026faf68fc44bdd6c88428b9f2d222
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58782473"
---
# <a name="macossystemextensiontypemapping-resource-type"></a>Tipo de recurso macOSSystemExtensionTypeMapping

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um mapeamento entre identificadores de equipe para extensões do sistema macOS e tipos de extensão do sistema.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|teamIdentifier|Cadeia de caracteres|Obtém ou define o identificador de equipe usado para assinar a extensão do sistema.|
|allowedTypes|[macOSSystemExtensionType](../resources/intune-deviceconfig-macossystemextensiontype.md)|Obtém ou define os tipos de extensão do sistema macOS permitidos. Os valores possíveis são: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtensionTypeMapping",
  "teamIdentifier": "String",
  "allowedTypes": "String"
}
```



