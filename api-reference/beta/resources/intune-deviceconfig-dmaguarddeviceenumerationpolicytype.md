---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f735a5ce77c0162899d7e93974a07de4f0be137b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469160"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>tipo de enumeração dmaGuardDeviceEnumerationPolicyType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis de DmaGuardDeviceEnumerationPolicy.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Valor padrão. Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.|
|blockAll|1|Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.|
|allowAll|duas|Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.|



