---
title: tipo de enumeração macOSContentCachingClientPolicy
description: Determina quais clientes um cache de conteúdo servirá.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ff1146d69fabdb8a9e734e0ae82747831e0a390
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026639"
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
|clientsInLocalNetwork|1 |Os caches de conteúdo fornecerão conteúdo aos dispositivos somente em sua rede local imediata.|
|clientsWithSamePublicIpAddress|2 |Os caches de conteúdo fornecerão conteúdo aos dispositivos que compartilham o mesmo endereço IP público.|
|clientsInCustomLocalNetworks|3 |Os caches de conteúdo fornecerão conteúdo aos dispositivos no contentCachingClientListenRanges.|
|clientsInCustomLocalNetworksWithFallback|4 |Os caches de conteúdo fornecerão conteúdo aos dispositivos no contentCachingClientListenRanges, contentCachingPeerListenRanges e contentCachingParents.|






