---
title: Tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c142829c41e518a61cd37300163a51751c281ce14a052b54e8bbeb9a2204f85e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185695"
---
# <a name="osversioncount-resource-type"></a>Tipo de recurso osVersionCount

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contagem de dispositivos com malware para cada versão do sistema operacional

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|osVersion|String|Versão do sistema operacional|
|deviceCount|Int32|Contagem de dispositivos com malware para a versão do sistema operacional|
|lastUpdateDateTime|DateTimeOffset|O Timestamp da última atualização para a contagem de dispositivos em UTC|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```




