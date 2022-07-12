---
title: Tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de pares
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a2e05fe9c378f14f1b60a0ac520301010c5ac5c
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730662"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>Tipo de enumeração windowsDeliveryOptimizationMode

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modo de otimização de entrega para distribuição de pares

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Userdefined|0|Permitir que o usuário defina.|
|httpOnly|1|HTTP apenas, sem emparelhamento|
|httpWithPeeringNat|2|Padrão do sistema operacional – Http combinado com emparelhamento por trás do mesmo tradutor de endereços de rede|
|httpWithPeeringPrivateGroup|3|HTTP combinado com emparelhamento em um grupo privado|
|httpWithInternetPeering|4|HTTP combinado com emparelhamento de Internet|
|simpleDownload|99|Modo de download simples sem emparelhamento|
|bypassMode|100|Modo de bypass. Não use a Otimização de Entrega e use BITS em vez disso|





