---
title: tipo de enum androidDeviceOwnerRequiredPasswordType
description: Política do proprietário do dispositivo Android necessários tipo de senha.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1208de597baff9dd05a48663435a3a928f3dae9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938038"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>tipo de enum androidDeviceOwnerRequiredPasswordType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Política do proprietário do dispositivo Android necessários tipo de senha.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Valor de padrão de dispositivo, sem intenção.|
|obrigatório|1|Deve haver um conjunto de senha, mas não existem restrições no tipo.|
|numéricos|2|AT menos numérico.|
|numericComplex|3|AT menos numérico com sequências de repetição ou ordenadas.|
|alfabético|4|Senha de pelo menos alfabética.|
|alfanumérico|5|Senha alfanumérica pelo menos|
|alphanumericWithSymbols|6|Pelo menos alfanumérico com símbolos.|





