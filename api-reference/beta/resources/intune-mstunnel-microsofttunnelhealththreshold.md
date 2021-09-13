---
title: Tipo de recurso microsoftTunnelHealthThreshold
description: Entidade que representa os limites de saúde de uma métrica de saúde.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6661fac1b2096f4164d81ce111032a0bb551dfdc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057289"
---
# <a name="microsofttunnelhealththreshold-resource-type"></a>Tipo de recurso microsoftTunnelHealthThreshold

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa os limites de saúde de uma métrica de saúde.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelHealthThresholds](../api/intune-mstunnel-microsofttunnelhealththreshold-list.md)|[coleção microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|Listar propriedades e relações dos [objetos microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|
|[Obter microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-get.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|Ler propriedades e relações do [objeto microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|
|[Criar microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-create.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|Crie um novo [objeto microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|
|[Excluir microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-delete.md)|Nenhum|Exclui um [microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md).|
|[Atualizar microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-update.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|Atualize as propriedades de [um objeto microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O nome métrico|
|healthyThreshold|Int64|O limite para estar saudável|
|unhealthyThreshold|Int64|O limite para não estar 100%|
|defaultHealthyThreshold|Int64|O limite padrão para ser saudável|
|defaultUnhealthyThreshold|Int64|O limite padrão para não estar 100%|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelHealthThreshold"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "id": "String (identifier)",
  "healthyThreshold": 1024,
  "unhealthyThreshold": 1024,
  "defaultHealthyThreshold": 1024,
  "defaultUnhealthyThreshold": 1024
}
```



