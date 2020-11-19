---
title: tipo de enumeração macOSContentCachingClientPolicy
description: Determina quais clientes um cache de conteúdo servirá.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8b2baeb66173b8e09f46bd570aa799ca9d2845e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268780"
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




