---
title: Tipo de recurso certificateConnectorDetails
description: Entidade usada para recuperar informações sobre conectores de certificado do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2dd74a003add77fffd029153fc9295b603ce3eef
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338950"
---
# <a name="certificateconnectordetails-resource-type"></a>Tipo de recurso certificateConnectorDetails

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade usada para recuperar informações sobre conectores de certificado do Intune.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar certificateConnectorDetailses](../api/intune-raimportcerts-certificateconnectordetails-list.md)|[Coleção certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|Listar propriedades e relações dos objetos [certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)|
|[Obter certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-get.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|Leia propriedades e relações do objeto [certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)|
|[Criar certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-create.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|Crie um novo [objeto certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)|
|[Excluir certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-delete.md)|Nenhum|Exclui um [certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md).|
|[Atualizar certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-update.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|Atualize as propriedades de [um objeto certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)|
|[Ação getHealthMetrics](../api/intune-raimportcerts-certificateconnectordetails-gethealthmetrics.md)|[Coleção keyLongValuePair](../resources/intune-shared-keylongvaluepair.md)|Ainda não documentado|
|[Ação getHealthMetricTimeSeries](../api/intune-raimportcerts-certificateconnectordetails-gethealthmetrictimeseries.md)|[Coleção certificateConnectorHealthMetricValue](../resources/intune-raimportcerts-certificateconnectorhealthmetricvalue.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para este conjunto de ConnectorDetails.|
|connectorName|String|Nome do conector (definido durante o registro).|
|machineName|String|Nome do computador que hospeda esse serviço de conector.|
|enrollmentDateTime|DateTimeOffset|Data/hora em que esse conector foi inscrito.|
|lastCheckinDateTime|DateTimeOffset|Data/hora em que esse conector se conectou pela última vez ao serviço.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.certificateConnectorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorDetails",
  "id": "String (identifier)",
  "connectorName": "String",
  "machineName": "String",
  "enrollmentDateTime": "String (timestamp)",
  "lastCheckinDateTime": "String (timestamp)"
}
```




