---
title: Tipo de número macOSContentCachingParentSelectionPolicy
description: Determina como os caches de conteúdo selecionam um cache pai.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ee647c2a6f6b2c4176ff042fe33e08f7cd0e0dca871f5e21b87c3e325faa6543
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206624"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a>Tipo de número macOSContentCachingParentSelectionPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Determina como os caches de conteúdo selecionam um cache pai.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Padrão para estratégia round-robin.|
|roundRobin|1 |Girar pelos pais em ordem. Use esta política para balanceamento de carga.|
|firstAvailable|2|Sempre use o primeiro pai disponível na lista Pais. Use essa política para designar pais primários, secundários e subsequentes permanentes.|
|urlPathHash|3 |Hash a parte do caminho da URL solicitada para que o mesmo pai seja sempre usado para a mesma URL. Isso é útil para maximizar o tamanho dos caches combinados dos pais.|
|random|4 |Escolha um pai aleatoriamente. Use esta política para balanceamento de carga.|
|stickyAvailable|5 |Use o primeiro pai disponível disponível na lista Pais até que ele fique indisponível e avance para o próximo. Use essa política para designar pais primários, secundários e subsequentes flutuantes.|




