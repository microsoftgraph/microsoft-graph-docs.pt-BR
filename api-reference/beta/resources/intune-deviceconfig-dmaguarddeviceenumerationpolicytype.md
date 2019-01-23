---
title: tipo de enum dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis a DmaGuardDeviceEnumerationPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429158"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>tipo de enum dmaGuardDeviceEnumerationPolicyType

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Valores possíveis a DmaGuardDeviceEnumerationPolicy.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Valor padrão. Dispositivos com DMA novo mapeamento drivers incompatíveis serão enumerados somente depois que o usuário desbloqueia a tela.|
|blockAll|1|Dispositivos com DMA novo mapeamento drivers incompatíveis nunca poderão iniciar e executar DMA a qualquer momento.|
|allowAll|2|Todos os DMA capaz PCIe dispositivos externos serão enumerados a qualquer momento.|




