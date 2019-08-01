---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 49fdf3172879092a04c20d0d73724744a9ef0fb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031560"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de enumeração firewallPacketQueueingMethodType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para firewallPacketQueueingMethod

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário|
|deficiência|1|Desabilitar enfileiramento de pacotes|
|queueInbound|duas|Enfileirar pacotes criptografados de entrada|
|queueOutbound|3D|Pacotes de saída de fila descriptografados para encaminhamento|
|queueBoth|quatro|Enfileiramento de pacotes de entrada e de saída|



