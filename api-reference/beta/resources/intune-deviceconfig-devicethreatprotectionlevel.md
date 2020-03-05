---
title: tipo de enumeração deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a06e0ba5c34198d181a8ba854cf20a16b1e2aeab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530107"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>tipo de enumeração deviceThreatProtectionLevel

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|indisponível|,0|Valor padrão. Não usar.|
|presos|1 |Requisito de nível de ameaça de dispositivo: protegido. Este é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.|
|low|2 |Requisito de nível de proteção contra ameaças de dispositivos: baixo. Low representa uma severidade de ameaça que representa o risco mínimo para os dados do dispositivo ou dispositivo.|
|medium|3 |Requisito de nível de proteção contra ameaças de dispositivos: médio. Médio representa uma severidade de ameaça que representa o risco moderado para os dados do dispositivo ou dispositivo.|
|high|4 |Requisito de nível de proteção contra ameaças de dispositivos: alto. High representa uma severidade de ameaça que representa sérios riscos nos dados do dispositivo ou dispositivo.|
|notSet|10 |Requisito de nível de proteção contra ameaças de dispositivos: não definido. Not set indica que não há necessidade de o dispositivo atender a um nível de proteção contra ameaças.|



