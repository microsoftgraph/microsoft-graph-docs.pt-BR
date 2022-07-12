---
title: Tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b3d3ad0ecc4951e6b8d38855c7a773fe2d6a4d4a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734309"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>Tipo de enumeração firewallPacketQueueingMethodType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallPacketQueueingMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|desabilitadas|1|Desabilitar o enfileiramento de pacotes|
|queueInbound|2|Enfileirar pacotes criptografados de entrada|
|queueOutbound|3|Fila de pacotes de saída descriptografados para encaminhamento|
|queueBoth|4|Enfileirar pacotes de entrada e saída|





