---
title: Tipo de número macOSSoftwareUpdateDelayPolicy
description: Número de sinalizador para determinar se as atualizações de software de atraso para macOS são demoradas.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 18ce0f39150b4b551b33f7c13dfc96817237617b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054503"
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



