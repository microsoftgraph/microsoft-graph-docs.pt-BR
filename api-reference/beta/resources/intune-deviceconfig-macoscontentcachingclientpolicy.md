---
title: Tipo de número macOSContentCachingClientPolicy
description: Determina quais clientes um cache de conteúdo servirá.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8bc8ab9be74dc9686ea534ae98ea170b4ed6760d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017495"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a>Tipo de número macOSContentCachingClientPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determina quais clientes um cache de conteúdo servirá.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Padrão para clientes na rede local.|
|clientsInLocalNetwork|1|Os caches de conteúdo fornecerão conteúdo apenas para dispositivos em sua rede local imediata.|
|clientsWithSamePublicIpAddress|2|Os caches de conteúdo fornecerão conteúdo para dispositivos que compartilham o mesmo endereço IP público.|
|clientsInCustomLocalNetworks|3|Os caches de conteúdo fornecerão conteúdo para dispositivos em contentCachingClientListenRanges.|
|clientsInCustomLocalNetworksWithFallback|4 |Os caches de conteúdo fornecerão conteúdo para dispositivos em contentCachingClientListenRanges, contentCachingPeerListenRanges e contentCachingParents.|



