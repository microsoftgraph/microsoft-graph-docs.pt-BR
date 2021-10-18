---
title: tipo de número firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f9303b2eb09ba9b9ea652a19726fd9c0b930bd79
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60449605"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de número firewallPacketQueueingMethodType

Namespace: microsoft.graph

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



