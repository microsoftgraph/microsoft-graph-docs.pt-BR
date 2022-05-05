---
title: Tipo de enumeração windowsAutopilotDeviceRemediationState
description: Status de correção do dispositivo, indicando se o hardware foi alterado ou não para um dispositivo registrado no Autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a6220236194bdb2bfbe655359cfc1d7291d90436
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210931"
---
# <a name="windowsautopilotdeviceremediationstate-enum-type"></a>Tipo de enumeração windowsAutopilotDeviceRemediationState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status de correção do dispositivo, indicando se o hardware foi alterado ou não para um dispositivo registrado no Autopilot.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Status desconhecido.|
|noRemediationRequired|1|Nenhuma alteração de hardware foi detectada.|
|automaticRemediationRequired|2|Alteração de hardware detectada no cliente. A correção adicional é necessária.|
|manualRemediationRequired|3|Alteração de hardware detectada no cliente que não pôde ser resolvida automaticamente. A correção adicional é necessária.|
|unknownFutureValue|4|Marca o final dos valores de enumeração conhecidos e permite valores adicionais no futuro.|




