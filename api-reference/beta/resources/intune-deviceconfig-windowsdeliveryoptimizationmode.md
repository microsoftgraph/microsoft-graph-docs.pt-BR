---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b2a66292ec6fb5db3fead93cbda7d24f5e505514
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371163"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>tipo de enumeração windowsDeliveryOptimizationMode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modo de otimização de entrega para distribuição de mesmo nível

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|httpOnly|1|Somente HTTP, sem emparelhamento|
|httpWithPeeringNat|duas|Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede|
|httpWithPeeringPrivateGroup|3D|HTTP combinado com emparelhamento em um grupo privado|
|httpWithInternetPeering|quatro|HTTP combinado com emparelhamento da Internet|
|simpleDownload|99|Modo de download simples sem emparelhamento|
|bypassmode|100|Modo bypass. Não usar otimização de entrega e usar BITS em vez disso|



