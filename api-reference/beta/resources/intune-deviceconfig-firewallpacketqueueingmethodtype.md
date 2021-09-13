---
title: tipo de número firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 02f89ecf96bb2d942389a73e96cd2b1f06eb35b8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064304"
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



