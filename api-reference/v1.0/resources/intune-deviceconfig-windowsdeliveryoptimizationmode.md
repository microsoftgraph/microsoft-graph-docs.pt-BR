---
title: Tipo denum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de pares
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5c483f00817858e7061bacf1b1e2b6ec6c00a02b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742745"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>Tipo denum windowsDeliveryOptimizationMode

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modo de otimização de entrega para distribuição de pares

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário desem conjunto.|
|httpOnly|1|Somente HTTP, sem par|
|httpWithPeeringNat|2|Padrão do sistema operacional – Http mesclado com o peering por trás do mesmo tradutor de endereços de rede|
|httpWithPeeringPrivateGroup|3|HTTP mesclado com o peering em um grupo privado|
|httpWithInternetPeering|4 |HTTP mesclado com o peering da Internet|
|simpleDownload|99|Modo de download simples sem par|
|bypassMode|100|Modo bypass. Não use a Otimização de Entrega e use BITS em vez disso|




