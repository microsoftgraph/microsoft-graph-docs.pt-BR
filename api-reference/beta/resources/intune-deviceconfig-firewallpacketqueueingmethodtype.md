---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aca93f0c7afaa0e7859ceccb73fad656f3590b1a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294449"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de enumeração firewallPacketQueueingMethodType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallPacketQueueingMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|desabilitadas|1|Desabilitar enfileiramento de pacotes|
|queueInbound|duas|Enfileirar pacotes criptografados de entrada|
|queueOutbound|3D|Pacotes de saída de fila descriptografados para encaminhamento|
|queueBoth|4 |Enfileiramento de pacotes de entrada e de saída|




