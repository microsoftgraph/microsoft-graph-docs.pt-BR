---
title: tipo de enum deviceThreatProtectionLevel
description: Níveis de proteção de ameaça de dispositivo para a API de proteção de ameaça do dispositivo.
ms.openlocfilehash: 9b6a5066c26dcfe5ee2922bc736cf0292b1d3055
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006905"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>tipo de enum deviceThreatProtectionLevel

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Níveis de proteção de ameaça de dispositivo para a API de proteção de ameaça do dispositivo.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|indisponível|0|Valor padrão. Não a use.|
|protegido|1|Requisito de dispositivo de nível de ameaça: protegido. Isso é o nível mais seguro e representa que nenhuma ameaça foram encontrada no dispositivo.|
|low|2|Requisito de nível de proteção contra ameaças de dispositivo: baixa. Baixa representa severidade ameaça que representa um risco mínimo para o dispositivo ou os dados do dispositivo.|
|medium|3|Requisito de nível de proteção contra ameaças de dispositivo: médio. Médio representa severidade ameaça que traz moderar risco ao dispositivo ou dados do dispositivo.|
|high|4|Requisito de nível de proteção contra ameaças de dispositivo: alta. Alta representa severidade ameaça que representa um risco severo para o dispositivo ou os dados do dispositivo.|
|notSet|10|Requisito de nível de proteção contra ameaças do dispositivo: não definido. Não set representa que não há nenhuma exigência para o dispositivo atender a um nível de proteção contra ameaças.|



