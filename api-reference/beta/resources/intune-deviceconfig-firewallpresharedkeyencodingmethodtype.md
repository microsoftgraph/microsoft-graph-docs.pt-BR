---
title: tipo de enum firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dd5eb58c4fe2e8729ab1adc4aa55ad0c701157f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862150"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>tipo de enum firewallPreSharedKeyEncodingMethodType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallPreSharedKeyEncodingMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|nenhum|1|Chave pré compartilhada não é codificado. Em vez disso, ele é mantido em seu formato de caractere largo|
|utF8|2|Codificar a chave pré compartilhada usando a codificação UTF-8|





