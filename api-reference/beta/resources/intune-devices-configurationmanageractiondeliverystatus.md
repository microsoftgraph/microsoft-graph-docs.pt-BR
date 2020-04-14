---
title: tipo de enumeração configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ab437ff9a7945b4bdd61b4e3e3a103e72b780e04
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465118"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>tipo de enumeração configurationManagerActionDeliveryStatus

Namespace: microsoft.graph

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



