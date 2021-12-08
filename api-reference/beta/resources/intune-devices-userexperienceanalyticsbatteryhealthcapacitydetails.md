---
title: tipo de recurso userExperienceAnalyticsBatteryHealthCapacityDetails
description: A entidade de capacidade da bateria de análise de experiência do usuário contém a contagem de dispositivos divididos em 3 categorias - dispositivos com capacidade > 80%, dispositivos com capacidade de 50 a 80% e dispositivos com capacidade < 50 %. Esta API fornece a contagem de dispositivos nessas três categorias..
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db0c5268b3f40ac726ca98336cb2a1ddf2e8cf9d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343151"
---
# <a name="userexperienceanalyticsbatteryhealthcapacitydetails-resource-type"></a>tipo de recurso userExperienceAnalyticsBatteryHealthCapacityDetails

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de capacidade da bateria de análise de experiência do usuário contém a contagem de dispositivos divididos em 3 categorias - dispositivos com capacidade > 80%, dispositivos com capacidade de 50 a 80% e dispositivos com capacidade < 50 %. Esta API fornece a contagem de dispositivos nessas três categorias..

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userExperienceAnalyticsBatteryHealthCapacityDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails-get.md)|[userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthCapacityDetails.](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md)|
|[Atualizar userExperienceAnalyticsBatteryHealthCapacityDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails-update.md)|[userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthCapacityDetails.](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de capacidade da bateria de análise de experiência do usuário.|
|activeDevices|Int32|Número de dispositivos ativos no locatário. Valores válidos -2147483648 para 2147483647|
|batteryCapacityGood|Int32|Número de dispositivos cuja capacidade máxima de bateria é maior do que 80%. Valores válidos -2147483648 para 2147483647|
|batteryCapacityFair|Int32|Número de dispositivos cuja capacidade máxima de bateria é maior do que 50% mas inferior a 80%. Valores válidos -2147483648 para 2147483647|
|batteryCapacityPoor|Int32|Número de dispositivos cuja capacidade máxima da bateria é inferior a 50%. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "batteryCapacityGood": 1024,
  "batteryCapacityFair": 1024,
  "batteryCapacityPoor": 1024
}
```




