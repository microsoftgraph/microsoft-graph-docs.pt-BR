---
title: tipo de enumeração macOSContentCachingPeerPolicy
description: Determina quais conteúdos em cache outros caches de conteúdo terão pontos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7305c42098782d9e69e734037fb08d3238c7b4a9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268745"
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
|peersInLocalNetwork|1|Os caches de conteúdo só serão iguais aos caches em sua rede local imediata.|
|peersWithSamePublicIpAddress|duas|Os caches de conteúdo só serão pontos com caches que compartilham o mesmo endereço IP público.|
|peersInCustomLocalNetworks|3D|Os caches de conteúdo usarão o contentCachingPeerFilterRanges e o contentCachingPeerListenRanges para determinar em que caches os pontos serão.|




