---
title: Tipo de número dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis do DmaGuardDeviceEnumerationPolicy.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 66a04e3288d9faaf34a42915ab03e859612e3fe9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59009186"
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
|blockAll|1|Os dispositivos com drivers incompatíveis de remapping DMA nunca terão permissão para iniciar e executar o DMA a qualquer momento.|
|allowAll|2|Todos os dispositivos PCIe compatíveis com DMA externos serão enumerados a qualquer momento.|



