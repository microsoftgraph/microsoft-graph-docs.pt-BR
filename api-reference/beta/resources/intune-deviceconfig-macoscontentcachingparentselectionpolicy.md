---
title: tipo de enumeração macOSContentCachingParentSelectionPolicy
description: Determina como os caches de conteúdo selecionam um cache pai.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0e618ee1a18083052e926a3193e941d61933afd7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268773"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a>tipo de enumeração macOSContentCachingParentSelectionPolicy

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determina como os caches de conteúdo selecionam um cache pai.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|O padrão é a estratégia de rodízio.|
|roundRobin|1|Girar através dos pais na ordem. Use esta política para balanceamento de carga.|
|firstAvailable|duas|Sempre use o primeiro pai disponível na lista de pais. Use essa política para designar os pais primários, secundários e subsequentes permanentes.|
|urlPathHash|3D|Hash a parte do caminho da URL solicitada para que o mesmo pai seja sempre usado para a mesma URL. Isso é útil para maximizar o tamanho dos caches combinados dos pais.|
|aleatório|4 |Escolha um pai aleatoriamente. Use esta política para balanceamento de carga.|
|stickyAvailable|5 |Use o primeiro pai disponível que está disponível na lista de pais até que fique indisponível e vá para o próximo. Use essa política para designar os pais primários, secundários e subsequentes.|




