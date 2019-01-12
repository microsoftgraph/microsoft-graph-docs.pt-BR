---
title: tipo de enum deviceThreatProtectionLevel
description: Níveis de proteção de ameaça de dispositivo para a API de proteção de ameaça do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38d4c17fc9883b23417a4c72ac7cc3c75512865c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948048"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>tipo de enum deviceThreatProtectionLevel

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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





