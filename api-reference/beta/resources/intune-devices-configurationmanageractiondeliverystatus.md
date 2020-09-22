---
title: tipo de enumeração configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1751f4e53c3df3b3a27d759ff9f747ead5360211
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060689"
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
|pendingDelivery|1 |Pendente para entregar a ação a ConfigurationManager|
|deliveredToConnectorService|2 |A ação é enviada para o serviço do conector ConfigurationManager (nuvem)|
|failedToDeliverToConnectorService|3 |Falha ao enviar a ação para o serviço do conector ConfigurationManager (nuvem)|
|deliveredToOnPremisesServer|4 |A ação é entregue no servidor local do ConfigurationManager|






