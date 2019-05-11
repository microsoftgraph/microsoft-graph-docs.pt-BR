---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94ff2a645b9ea3862cee50ca086284deea02da09
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942014"
---
# <a name="deviceregistrationstate-enum-type"></a>tipo de enumeração deviceRegistrationState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Não registrado|,0|O dispositivo não está registrado.|
|inscreve|duas|O dispositivo está registrado.|
|revogado|3D|O dispositivo foi bloqueado, apagado ou desativado.|
|keyconflict|quatro|O dispositivo tem um conflito de teclas.|
|approvalPending|0,5|O dispositivo está aguardando aprovação.|
|certificateReset|6|O certificado de dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|178|O dispositivo não está registrado e registro pendente.|
|desconhecido|8 |O status do registro do dispositivo é desconhecido.|




