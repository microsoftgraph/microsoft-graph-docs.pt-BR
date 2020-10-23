---
title: tipo de enumeração macOSContentCachingClientPolicy
description: Determina quais clientes um cache de conteúdo servirá.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c6900fbc3f1e5c76fb11eed68a349438ead24f48
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735826"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a>tipo de enumeração macOSContentCachingClientPolicy

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determina quais clientes um cache de conteúdo servirá.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|O padrão é para os clientes na rede local.|
|clientsInLocalNetwork|1|Os caches de conteúdo fornecerão conteúdo aos dispositivos somente em sua rede local imediata.|
|clientsWithSamePublicIpAddress|duas|Os caches de conteúdo fornecerão conteúdo aos dispositivos que compartilham o mesmo endereço IP público.|
|clientsInCustomLocalNetworks|3D|Os caches de conteúdo fornecerão conteúdo aos dispositivos no contentCachingClientListenRanges.|
|clientsInCustomLocalNetworksWithFallback|4 |Os caches de conteúdo fornecerão conteúdo aos dispositivos no contentCachingClientListenRanges, contentCachingPeerListenRanges e contentCachingParents.|





