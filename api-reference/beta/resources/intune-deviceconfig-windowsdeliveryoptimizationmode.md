---
title: Tipo denum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de pares
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7ee5580f22244b498803d925ca61f4d71f193298
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033627"
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



