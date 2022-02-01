---
title: Tipo de recurso oemWarranty
description: Informações sobre a Garantia do OEM para um determinado dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e64e0018fc185cfb79ecc32990b6c4ad4b02c7d
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292258"
---
# <a name="oemwarranty-resource-type"></a>Tipo de recurso oemWarranty

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações sobre a Garantia do OEM para um determinado dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|baseWarranties|[Coleção warrantyOffer](../resources/intune-devices-warrantyoffer.md)|Lista de ofertas de garantia base. Essa coleção pode conter no máximo 100 elementos.|
|additionalWarranties|[Coleção warrantyOffer](../resources/intune-devices-warrantyoffer.md)|Lista de ofertas adicionais de garantia. Essa coleção pode conter no máximo 100 elementos.|
|deviceWarrantyUrl|String|URL da página de garantia do dispositivo|
|deviceConfigurationUrl|Cadeia de caracteres|URL da página de configuração do dispositivo|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oemWarranty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oemWarranty",
  "baseWarranties": [
    {
      "@odata.type": "microsoft.graph.warrantyOffer",
      "type": "String",
      "description": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)"
    }
  ],
  "additionalWarranties": [
    {
      "@odata.type": "microsoft.graph.warrantyOffer",
      "type": "String",
      "description": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)"
    }
  ],
  "deviceWarrantyUrl": "String",
  "deviceConfigurationUrl": "String"
}
```




