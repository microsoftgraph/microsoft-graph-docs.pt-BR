---
title: tipo de enum vppTokenActionFailureReason
description: Tipos possíveis razões para uma falha de token de ação do programa de compra de Volume do Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: baf33c29a822cc725c66ff6a3a7d796e57e63693
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961159"
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





