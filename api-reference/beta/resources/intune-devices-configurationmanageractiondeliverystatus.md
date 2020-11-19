---
title: tipo de enumeração configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bbe36a6f7e346467d35bf997817241d7f30ef6df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214621"
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




