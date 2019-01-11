---
title: tipo de enum vppTokenActionFailureReason
description: Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f488302b7fc701e8a419357ad7d6cbbb6015759b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883717"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>tipo de enum vppTokenActionFailureReason

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhum|0|Nenhum.|
|appleFailure|1|Houve um erro no serviço da Apple.|
|internalError|2|Houve um erro interno.|
|expiredVppToken|3|Houve um erro, porque o token do programa de compra de Volume do Apple expirou.|
|expiredApplePushNotificationCertificate|4|Houve um erro, porque o certificado de notificação de Push do Apple Volume compra programa expirado.|





