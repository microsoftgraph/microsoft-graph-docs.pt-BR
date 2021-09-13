---
title: tipo de número configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Configuration Manager
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e776d03e4d785191ff3463bae125d786250ee22d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111002"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>tipo de número configurationManagerActionDeliveryStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de entrega da ação de dispositivo do Configuration Manager

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Pendente para entregar a ação ao ConfigurationManager|
|pendingDelivery|1|Pendente para entregar a ação ao ConfigurationManager|
|deliveredToConnectorService|2|A ação é enviada para o serviço ConfigurationManager Connector (nuvem)|
|failedToDeliverToConnectorService|3|Falha ao enviar a ação para o serviço ConfigurationManager Connector (nuvem)|
|deliveredToOnPremisesServer|4 |A ação é entregue ao servidor configurationManager no local|



