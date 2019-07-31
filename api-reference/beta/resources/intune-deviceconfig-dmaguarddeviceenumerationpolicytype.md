---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 00bf6986f37bd5fd1aae4991dbb7eb5b215e4c6e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001541"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>tipo de enumeração dmaGuardDeviceEnumerationPolicyType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis de DmaGuardDeviceEnumerationPolicy.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Valor padrão. Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.|
|blockAll|1|Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.|
|allowAll|duas|Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.|





