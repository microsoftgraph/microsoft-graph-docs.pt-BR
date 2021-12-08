---
title: Tipo de número macOSSoftwareUpdateDelayPolicy
description: Número de sinalizador para determinar se as atualizações de software de atraso para macOS são demoradas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dc7fa44a86f4b10ca3f49172b86ee3bfdb336da8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339889"
---
# <a name="macossoftwareupdatedelaypolicy-enum-type"></a>Tipo de número macOSSoftwareUpdateDelayPolicy

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Número de sinalizador para determinar se as atualizações de software de atraso para macOS são demoradas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Os atrasos de atualização de software não serão imposto.|
|delayOSUpdateVisibility|1|Forçar atrasos para atualizações de software do sistema operacional.|
|delayAppUpdateVisibility|2|Force delays for app software updates.|
|unknownFutureValue|4|Membro do Sentinel para casos em que o cliente não pode manipular os novos valores de numeração.|
|delayMajorOsUpdateVisibility|8 |Forçar atrasos para atualizações principais de software do sistema operacional.|




