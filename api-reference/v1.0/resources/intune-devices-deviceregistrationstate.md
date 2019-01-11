---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e2b755d213d39beb228afe603b2066b55416f14c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857320"
---
# <a name="deviceregistrationstate-enum-type"></a>tipo de enum deviceRegistrationState

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Status do registro do dispositivo.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notRegistered|0|O dispositivo não está registrado.|
|registrado|2|O dispositivo está registrado.|
|revogado|3|O dispositivo foi bloqueado, apagado ou desativado.|
|keyConflict|4|O dispositivo tem um conflito de chave.|
|approvalPending|5|O dispositivo está aguardando aprovação.|
|certificateReset|6|O certificado do dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|7|O dispositivo não está registrado e pendentes de inscrição.|
|unknown|8|O status do registro de dispositivo é desconhecido.|



