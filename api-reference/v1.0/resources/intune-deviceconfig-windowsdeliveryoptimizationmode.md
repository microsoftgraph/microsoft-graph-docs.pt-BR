---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 869c902e8fc0b02fed1037d1d1273d8584ece9fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530371"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>tipo de enumeração windowsDeliveryOptimizationMode

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modo de otimização de entrega para distribuição de mesmo nível

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|httpOnly|1 |Somente HTTP, sem emparelhamento|
|httpWithPeeringNat|2 |Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede|
|httpWithPeeringPrivateGroup|3 |HTTP combinado com emparelhamento em um grupo privado|
|httpWithInternetPeering|4 |HTTP combinado com emparelhamento da Internet|
|simpleDownload|99|Modo de download simples sem emparelhamento|
|bypassmode|100|Modo bypass. Não usar otimização de entrega e usar BITS em vez disso|




