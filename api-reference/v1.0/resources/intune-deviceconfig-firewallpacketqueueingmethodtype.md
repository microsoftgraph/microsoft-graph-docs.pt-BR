---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd9dc0279abc332bbf7b686f7f429fbd8db8883
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541305"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de enumeração firewallPacketQueueingMethodType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallPacketQueueingMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|deficiência|1 |Desabilitar enfileiramento de pacotes|
|queueInbound|2 |EnFileirar pacotes criptografados de entrada|
|queueOutbound|3 |Pacotes de saída de fila descriptografados para encaminhamento|
|queueBoth|4 |EnFileiramento de pacotes de entrada e de saída|



