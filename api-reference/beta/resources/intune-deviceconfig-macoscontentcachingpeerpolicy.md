---
title: tipo de enumeração macOSContentCachingPeerPolicy
description: Determina quais conteúdos em cache outros caches de conteúdo terão pontos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1f55bd6aafffc7602632155e4fa3c387c888aae9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735810"
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





