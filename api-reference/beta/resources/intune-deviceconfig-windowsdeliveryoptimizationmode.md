---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 719e315f8cccf52f98dfddb979d9f0fd5490dff8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692426"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>tipo de enumeração windowsDeliveryOptimizationMode

Namespace: microsoft.graph

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





