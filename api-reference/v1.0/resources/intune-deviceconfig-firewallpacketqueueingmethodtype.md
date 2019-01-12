---
title: tipo de enum firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3700df6d2eaf0dd0d2dde8a3f4a90be2e3684951
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940096"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de enum firewallPacketQueueingMethodType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallPacketQueueingMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|desabilitado|1|Desabilitar o serviço de enfileiramento de pacotes|
|queueInbound|2|Os pacotes criptografados entrados de fila|
|queueOutbound|3|Fila descriptografados para encaminhamento de pacotes de saída|
|queueBoth|4|Pacotes de entrada e saídos da fila|



