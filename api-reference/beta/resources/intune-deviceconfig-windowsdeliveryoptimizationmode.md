---
title: tipo de enum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de ponto
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 004bb3d3984d8d304f89dc339899035d218546a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972653"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>tipo de enum windowsDeliveryOptimizationMode

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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





