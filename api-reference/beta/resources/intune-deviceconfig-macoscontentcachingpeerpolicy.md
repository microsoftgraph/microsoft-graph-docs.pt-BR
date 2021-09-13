---
title: Tipo denum macOSContentCachingPeerPolicy
description: Determina com quais caches de conteúdo outros caches de conteúdo serão correspondentes.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 89ad8ff2865e31b7d1ef1789093fe123e44f2e14
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017489"
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



