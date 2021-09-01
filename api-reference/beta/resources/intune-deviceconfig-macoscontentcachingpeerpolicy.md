---
title: Tipo denum macOSContentCachingPeerPolicy
description: Determina com quais caches de conteúdo outros caches de conteúdo serão correspondentes.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22adc6cd2df6dad85875deb190f40c305776a991
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783544"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a>Tipo denum macOSContentCachingPeerPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determina com quais caches de conteúdo outros caches de conteúdo serão correspondentes.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Padrão para pares na rede local.|
|peersInLocalNetwork|1|Os caches de conteúdo só serão correspondentes aos caches em sua rede local imediata.|
|peersWithSamePublicIpAddress|2|Os caches de conteúdo só serão correspondentes a caches que compartilham o mesmo endereço IP público.|
|peersInCustomLocalNetworks|3|Os caches de conteúdo usarão contentCachingPeerFilterRanges e contentCachingPeerListenRanges para determinar com quais caches fazer par.|



