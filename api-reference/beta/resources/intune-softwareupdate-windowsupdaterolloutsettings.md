---
title: Tipo de recurso windowsUpdateRolloutSettings
description: Um tipo complexo para armazenar as configurações de lançamento de atualizações do Windows, incluindo a hora da data de início da oferta, a data de término e os dias entre cada conjunto de ofertas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d0d6849fcb41be6493f11a6d1b3d01c8409e9d6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688231"
---
# <a name="windowsupdaterolloutsettings-resource-type"></a>Tipo de recurso windowsUpdateRolloutSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar as configurações de lançamento de atualizações do Windows, incluindo a hora da data de início da oferta, a data de término e os dias entre cada conjunto de ofertas.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|offerStartDateTimeInUTC|DateTimeOffset|A data e a hora inicial da atualização de recursos a serem definidas, atualizadas e exibidas para um perfil de atualização de recursos, por exemplo: 2020-06-09T10:00:00Z.|
|offerEndDateTimeInUTC|DateTimeOffset|A atualização de recursos termina a data e hora de lançamento a serem definidas, atualizadas e exibidas para um perfil de atualização de recursos, por exemplo: 2020-06-09T10:00:00Z.|
|offerIntervalInDays|Int32|O número de dias entre cada conjunto de ofertas a serem definidas, atualizadas e exibidas para um perfil de atualização de recursos, por exemplo: se OfferStartDateTimeInUTC for 2020-06-09T10:00:00Z, e OfferIntervalInDays é 1, em seguida, os próximos dois conjuntos de ofertas serão feitos consecutivamente em 2020-06-10T10:00:00Z (próximo dia no mesmo horário especificado) e 2020-06-11T10:00:00Z (próximo dia no mesmo horário especificado) com 1 dia entre cada conjunto de ofertas.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateRolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateRolloutSettings",
  "offerStartDateTimeInUTC": "String (timestamp)",
  "offerEndDateTimeInUTC": "String (timestamp)",
  "offerIntervalInDays": 1024
}
```



