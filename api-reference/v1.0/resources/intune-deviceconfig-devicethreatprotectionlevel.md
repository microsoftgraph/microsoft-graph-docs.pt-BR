---
title: Tipo de enumeração deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças do dispositivo para a API de Proteção contra Ameaças do Dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 55b2cc465f33312fe939f9c2c826846a94bce2eb
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735738"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>Tipo de enumeração deviceThreatProtectionLevel

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Níveis de proteção contra ameaças do dispositivo para a API de Proteção contra Ameaças do Dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Indisponível|0|Valor Padrão. Não usar.|
|Seguro|1|Requisito de nível de ameaça do dispositivo: protegido. Esse é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.|
|low|2|Requisito de nível de Proteção contra Ameaças do Dispositivo: Baixo. Baixo representa uma severidade de ameaça que representa risco mínimo para os dados do dispositivo ou do dispositivo.|
|medium|3|Requisito de nível de Proteção contra Ameaças do Dispositivo: Médio. Médio representa uma severidade de ameaça que representa um risco moderado para os dados do dispositivo ou do dispositivo.|
|high|4|Requisito de nível de Proteção contra Ameaças do Dispositivo: Alto. Alta representa uma severidade de ameaça que representa um risco grave para os dados do dispositivo ou do dispositivo.|
|Notset|10|Requisito de nível de Proteção contra Ameaças do Dispositivo: Não Definido. Não definido representa que não há nenhum requisito para que o dispositivo atenda a um nível de Proteção contra Ameaças.|





