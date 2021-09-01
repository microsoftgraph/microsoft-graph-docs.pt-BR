---
title: Tipo de número macOSSoftwareUpdateDelayPolicy
description: Número de sinalizador para determinar se as atualizações de software de atraso para macOS são demoradas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 16204557d18024d40336b0f73a401141bf48c01a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791519"
---
# <a name="macossoftwareupdatedelaypolicy-enum-type"></a>Tipo de número macOSSoftwareUpdateDelayPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Número de sinalizador para determinar se as atualizações de software de atraso para macOS são demoradas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Os atrasos de atualização de software não serão imposto.|
|delayOSUpdateVisibility|1|Forçar atrasos para atualizações de software do sistema operacional.|
|delayAppUpdateVisibility|2|Force delays for app software updates.|
|unknownFutureValue|4 |Membro do Sentinel para casos em que o cliente não pode manipular os novos valores de numeração.|
|delayMajorOsUpdateVisibility|8 |Forçar atrasos para atualizações principais de software do sistema operacional.|



