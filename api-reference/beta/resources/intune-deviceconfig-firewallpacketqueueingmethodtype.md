---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b134e00e0237e407331f0ea0554c54dcf0d39ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529988"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de enumeração firewallPacketQueueingMethodType

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

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



