---
title: tipo de enumeração macOSContentCachingParentSelectionPolicy
description: Determina como os caches de conteúdo selecionam um cache pai.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 726c6d4feb7387fd67583c451a9f3399a316f4a0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735817"
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





