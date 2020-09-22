---
title: tipo de enumeração macOSContentCachingPeerPolicy
description: Determina quais conteúdos em cache outros caches de conteúdo terão pontos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e45f6d0e92624693139cd09ca4eff52cd483b46c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993823"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a>tipo de enumeração macOSContentCachingPeerPolicy

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determina quais conteúdos em cache outros caches de conteúdo terão pontos.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|O padrão é para pares na rede local.|
|peersInLocalNetwork|1 |Os caches de conteúdo só serão iguais aos caches em sua rede local imediata.|
|peersWithSamePublicIpAddress|2 |Os caches de conteúdo só serão pontos com caches que compartilham o mesmo endereço IP público.|
|peersInCustomLocalNetworks|3 |Os caches de conteúdo usarão o contentCachingPeerFilterRanges e o contentCachingPeerListenRanges para determinar em que caches os pontos serão.|






