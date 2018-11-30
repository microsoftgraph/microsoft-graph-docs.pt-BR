---
title: tipo de enum firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
ms.openlocfilehash: 70643e300f1a6cc151edeae849e5ae7c5f977750
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005638"
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



