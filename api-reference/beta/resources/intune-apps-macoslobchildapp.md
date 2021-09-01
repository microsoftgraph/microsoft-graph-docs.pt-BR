---
title: Tipo de recurso macOSLobChildApp
description: Contém propriedades do Aplicativo LOB do MacOS em um pacote de pacotes
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9518d975247f0ed3399524ca7c6d98839cadea9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58804880"
---
# <a name="macoslobchildapp-resource-type"></a>Tipo de recurso macOSLobChildApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades do Aplicativo LOB do MacOS em um pacote de pacotes

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleId|String|O Nome da Identidade.|
|buildNumber|String|O número de composição do aplicativo MacOS Line of Business (LoB).|
|versionNumber|String|O número de versão do aplicativo MacOS Line of Business (LoB).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```



