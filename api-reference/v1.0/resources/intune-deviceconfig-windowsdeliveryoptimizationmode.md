---
title: tipo de enum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de ponto
ms.openlocfilehash: 2d393a82f855f3e3a0226c8ccb450fa2dae1a95c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004823"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>tipo de enum windowsDeliveryOptimizationMode

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Modo de otimização de entrega para distribuição de ponto
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário pode definir.|
|httpOnly|1|HTTP apenas, nenhuma correspondência|
|httpWithPeeringNat|2|Padrão do sistema operacional – Http misturados com correspondência atrás do mesmo conversor de endereços de rede|
|httpWithPeeringPrivateGroup|3|HTTP misturados com correspondência entre um grupo privado|
|httpWithInternetPeering|4|HTTP misturado com correspondência de Internet|
|simpleDownload|99|Modo de download simples com nenhuma correspondência|
|bypassMode|100|Modo de desvio. Não use a otimização de entrega e usar o BITS|



