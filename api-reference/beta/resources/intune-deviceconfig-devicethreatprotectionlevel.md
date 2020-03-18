---
title: tipo de enumeração deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aa69e2e4d2122a8611a0db6a277dbfd5085561ba
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791986"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>tipo de enumeração deviceThreatProtectionLevel

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|indisponível|,0|Valor padrão. Não usar.|
|presos|1|Requisito de nível de ameaça de dispositivo: protegido. Este é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.|
|low|duas|Requisito de nível de proteção contra ameaças de dispositivos: baixo. Low representa uma severidade de ameaça que representa o risco mínimo para os dados do dispositivo ou dispositivo.|
|medium|3D|Requisito de nível de proteção contra ameaças de dispositivos: médio. Médio representa uma severidade de ameaça que representa o risco moderado para os dados do dispositivo ou dispositivo.|
|high|4 |Requisito de nível de proteção contra ameaças de dispositivos: alto. High representa uma severidade de ameaça que representa sérios riscos nos dados do dispositivo ou dispositivo.|
|notSet|10 |Requisito de nível de proteção contra ameaças de dispositivos: não definido. Not set indica que não há necessidade de o dispositivo atender a um nível de proteção contra ameaças.|



