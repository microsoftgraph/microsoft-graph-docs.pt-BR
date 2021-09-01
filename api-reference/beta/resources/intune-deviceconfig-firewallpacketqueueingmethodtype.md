---
title: tipo de número firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b496651cb8735a06afd5ae68e56e4078095180dc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817100"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de número firewallPacketQueueingMethodType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallPacketQueueingMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|desabilitadas|1|Desabilitar a fila de pacotes|
|queueInbound|2|Fila de pacotes criptografados de entrada|
|queueOutbound|3|Pacotes de saída descriptografados da fila para encaminhamento|
|queueBoth|4 |Fila de pacotes de entrada e de saída|



