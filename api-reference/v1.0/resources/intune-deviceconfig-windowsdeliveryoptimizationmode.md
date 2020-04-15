---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9be3f6861076bed1ef2e6d45336d975c07cba576
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451484"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>tipo de enumeração windowsDeliveryOptimizationMode

Namespace: microsoft.graph

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







