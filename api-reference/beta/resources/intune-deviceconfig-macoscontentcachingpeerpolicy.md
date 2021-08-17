---
title: Tipo denum macOSContentCachingPeerPolicy
description: Determina com quais caches de conteúdo outros caches de conteúdo serão correspondentes.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b89b7043ca64f106ec1d3bbded041ae15461195c916db0d31cf32dd848d42e40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54181192"
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
|peersInLocalNetwork|1 |Os caches de conteúdo só serão correspondentes aos caches em sua rede local imediata.|
|peersWithSamePublicIpAddress|2|Os caches de conteúdo só serão correspondentes a caches que compartilham o mesmo endereço IP público.|
|peersInCustomLocalNetworks|3 |Os caches de conteúdo usarão contentCachingPeerFilterRanges e contentCachingPeerListenRanges para determinar com quais caches fazer par.|




