---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
ms.openlocfilehash: a622613bd4ca5e065c3d9eb0331c05c360c1837c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360540"
---
# <a name="deviceregistrationstate-enum-type"></a>tipo de enum deviceRegistrationState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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





