---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0b5976d7ff06620db9958dacdfdd0b8b0c81a191
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530723"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de enumeração firewallPacketQueueingMethodType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallPacketQueueingMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|deficiência|1 |Desabilitar enfileiramento de pacotes|
|queueInbound|2 |Enfileirar pacotes criptografados de entrada|
|queueOutbound|3 |Pacotes de saída de fila descriptografados para encaminhamento|
|queueBoth|4 |Enfileiramento de pacotes de entrada e de saída|




