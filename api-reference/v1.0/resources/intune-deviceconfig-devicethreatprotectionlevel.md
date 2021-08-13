---
title: Tipo de número deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivo para a API de Proteção contra Ameaças de Dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3765e3cbdd8ea1ae40183d621a7ff0fb352ba19fcfa58b27201b5eb62b4e20ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163779"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>Tipo de número deviceThreatProtectionLevel

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Níveis de proteção contra ameaças de dispositivo para a API de Proteção contra Ameaças de Dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unavailable|0|Valor padrão. Não usar.|
|secured|1|Requisito de Nível de Ameaça de Dispositivo: Protegido. Esse é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.|
|low|2|Requisito de nível de Proteção contra Ameaças de Dispositivo: Baixo. Baixo representa uma gravidade de ameaça que representa risco mínimo para os dados do dispositivo ou do dispositivo.|
|medium|3|Requisito de nível de Proteção contra Ameaças de Dispositivo: Médio. Médio representa uma gravidade de ameaça que representa um risco moderado para os dados do dispositivo ou do dispositivo.|
|high|4 |Requisito de nível de Proteção contra Ameaças de Dispositivo: Alto. Alta representa uma gravidade de ameaça que representa um risco grave para os dados do dispositivo ou do dispositivo.|
|notSet|10 |Requisito de nível de Proteção contra Ameaças de Dispositivo: Não Definido. Não definido representa que não há requisito para o dispositivo atender a um nível de Proteção contra Ameaças.|




