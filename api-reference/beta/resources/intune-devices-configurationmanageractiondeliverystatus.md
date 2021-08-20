---
title: tipo de número configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cda8bbb7f52898ddd042b8cba88b204907bfe9edff006510a61b6b36c7db66eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239410"
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
|pendingDelivery|1 |Pendente para entregar a ação ao ConfigurationManager|
|deliveredToConnectorService|2|A ação é enviada para o serviço ConfigurationManager Connector (nuvem)|
|failedToDeliverToConnectorService|3 |Falha ao enviar a ação para o serviço ConfigurationManager Connector (nuvem)|
|deliveredToOnPremisesServer|4 |A ação é entregue ao servidor configurationManager no local|




