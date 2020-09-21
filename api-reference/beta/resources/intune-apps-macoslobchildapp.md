---
title: tipo de recurso macOSLobChildApp
description: Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3eb06ecc8937fd8f2d6c8d74cd0aaf560a22b89c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989455"
---
# <a name="macoslobchildapp-resource-type"></a>tipo de recurso macOSLobChildApp

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleId|String|O Nome da Identidade.|
|buildNumber|String|O número de compilação do aplicativo de linha de negócios (LoB) MacOS.|
|versionNumber|String|O número da versão do aplicativo de linha de negócios (LoB) MacOS.|

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






