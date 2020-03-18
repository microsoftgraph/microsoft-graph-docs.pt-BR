---
title: tipo de enumeração configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Gerenciador de configurações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58dca2b1ecb5419a3f56889a55c0816f492af430
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785088"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>tipo de enumeração configurationManagerActionDeliveryStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de entrega da ação de dispositivo do Gerenciador de configurações

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Pendente para entregar a ação a ConfigurationManager|
|pendingDelivery|1|Pendente para entregar a ação a ConfigurationManager|
|deliveredToConnectorService|duas|A ação é enviada para o serviço do conector ConfigurationManager (nuvem)|
|failedToDeliverToConnectorService|3D|Falha ao enviar a ação para o serviço do conector ConfigurationManager (nuvem)|
|deliveredToOnPremisesServer|4 |A ação é entregue no servidor local do ConfigurationManager|



