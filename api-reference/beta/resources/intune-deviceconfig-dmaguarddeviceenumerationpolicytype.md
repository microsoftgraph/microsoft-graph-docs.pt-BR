---
title: Tipo de número dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis do DmaGuardDeviceEnumerationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f6899594f226c7d5515d79464d9c80e7a90a2f84c40196804e2015fb832369f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124756"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>Tipo de número dmaGuardDeviceEnumerationPolicyType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis do DmaGuardDeviceEnumerationPolicy.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Valor padrão. Os dispositivos com drivers incompatíveis de remapping DMA só serão enumerados depois que o usuário desbloquear a tela.|
|blockAll|1 |Os dispositivos com drivers incompatíveis de remapping DMA nunca terão permissão para iniciar e executar o DMA a qualquer momento.|
|allowAll|2|Todos os dispositivos PCIe compatíveis com DMA externos serão enumerados a qualquer momento.|




