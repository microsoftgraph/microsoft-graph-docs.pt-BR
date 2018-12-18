---
title: tipo de enum vppTokenActionFailureReason
description: Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.
author: tfitzmac
ms.openlocfilehash: f36b92238b097f50990bbdb2f3c3584b2ff48901
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320957"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>tipo de enum vppTokenActionFailureReason

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Nenhum.|
|appleFailure|1|Houve um erro no serviço da Apple.|
|internalError|2|Houve um erro interno.|
|expiredVppToken|3|Houve um erro, porque o token do programa de compra de Volume do Apple expirou.|
|expiredApplePushNotificationCertificate|4|Houve um erro, porque o certificado de notificação de Push do Apple Volume compra programa expirado.|





