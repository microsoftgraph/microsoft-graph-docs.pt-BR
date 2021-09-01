---
title: Tipo denum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de pares
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 83f5b5e4a3db00a4ef1459ff35aa0f438a118157
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818102"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>Tipo denum windowsDeliveryOptimizationMode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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



