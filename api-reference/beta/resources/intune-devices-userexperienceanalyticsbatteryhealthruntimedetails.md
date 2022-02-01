---
title: tipo de recurso userExperienceAnalyticsBatteryHealthRuntimeDetails
description: A entidade de tempo de execução de bateria de análise de experiência do usuário contém a contagem de dispositivos divididos em 3 categorias - dispositivos com tempo de execução > 5 horas, dispositivos com tempo de execução de 3 a 5 horas e dispositivos com tempo de execução < 3 horas. Esta API fornece a contagem de dispositivos nessas três categorias.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4328abe87c73c10d0b5e16a2b9869b539d168a62
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292064"
---
# <a name="userexperienceanalyticsbatteryhealthruntimedetails-resource-type"></a>tipo de recurso userExperienceAnalyticsBatteryHealthRuntimeDetails

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de tempo de execução de bateria de análise de experiência do usuário contém a contagem de dispositivos divididos em 3 categorias - dispositivos com tempo de execução > 5 horas, dispositivos com tempo de execução de 3 a 5 horas e dispositivos com tempo de execução < 3 horas. Esta API fornece a contagem de dispositivos nessas três categorias.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userExperienceAnalyticsBatteryHealthRuntimeDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails-get.md)|[userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md) .|
|[Atualizar userExperienceAnalyticsBatteryHealthRuntimeDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails-update.md)|[userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de tempo de execução da bateria de análise de experiência do usuário.|
|activeDevices|Int32|Número de dispositivos ativos no locatário. Valores válidos -2147483648 para 2147483647|
|batteryRuntimeGood|Int32|Número de dispositivos cujo tempo de execução ativo é maior do que 5 horas. Valores válidos -2147483648 para 2147483647|
|batteryRuntimeFair|Int32|Número de dispositivos cujo tempo de execução ativo é maior do que 3 horas, mas menor que 5 horas. Valores válidos -2147483648 para 2147483647|
|batteryRuntimePoor|Int32|Número de dispositivos cujo tempo de execução ativo é inferior a 3 horas. Valores válidos -2147483648 para 2147483647|
|lastRefreshedDateTime|DateTimeOffset|Hora da data registrada dessa instância de detalhes do tempo de execução.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "batteryRuntimeGood": 1024,
  "batteryRuntimeFair": 1024,
  "batteryRuntimePoor": 1024,
  "lastRefreshedDateTime": "String (timestamp)"
}
```




