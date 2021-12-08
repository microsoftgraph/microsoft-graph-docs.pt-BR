---
title: Tipo denum remoteAssistanceSessionType
description: 'Tipo da sessão de assistência remota realizada. Os valores possíveis são: `viewOnly` , `fullControl`'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ca39d756bc134a7210c504dbf624f9267d0fc042
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338131"
---
# <a name="remoteassistancesessiontype-enum-type"></a>Tipo denum remoteAssistanceSessionType

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo da sessão de assistência remota realizada. Os valores possíveis são: `viewOnly` , `fullControl`

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|viewOnly|0|Esse status indica uma sessão de exibição somente entre o auxiliar e o sharer.|
|fullControl|1|Esse status indica uma sessão em que o auxiliar foi capaz de assumir o controle total do dispositivo do sharer.|
|elevation|2|Esse status indica uma sessão em que o auxiliar foi capaz de tomar ações administrativas no dispositivo do sharer.|




