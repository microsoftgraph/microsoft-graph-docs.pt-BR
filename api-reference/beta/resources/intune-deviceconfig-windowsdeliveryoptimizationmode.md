---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: faf70d8cb1122b09d5fcc6a5dcbf221cf3a6991c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786513"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>tipo de enumeração windowsDeliveryOptimizationMode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modo de otimização de entrega para distribuição de mesmo nível

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|httpOnly|1|Somente HTTP, sem emparelhamento|
|httpWithPeeringNat|duas|Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede|
|httpWithPeeringPrivateGroup|3D|HTTP combinado com emparelhamento em um grupo privado|
|httpWithInternetPeering|4 |HTTP combinado com emparelhamento da Internet|
|simpleDownload|99|Modo de download simples sem emparelhamento|
|bypassmode|100|Modo bypass. Não usar otimização de entrega e usar BITS em vez disso|



