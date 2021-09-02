---
title: Tipo denum remoteAssistanceSessionType
description: 'Tipo da sessão de assistência remota realizada. Os valores possíveis são: `viewOnly` , `fullControl`'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4aea876b672a71e9bc82e9eea620d257c3c5ea01
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794292"
---
# <a name="remoteassistancesessiontype-enum-type"></a>Tipo denum remoteAssistanceSessionType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo da sessão de assistência remota realizada. Os valores possíveis são: `viewOnly` , `fullControl`

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|viewOnly|0|Esse status indica uma sessão de exibição somente entre o auxiliar e o sharer.|
|fullControl|1|Esse status indica uma sessão em que o auxiliar foi capaz de assumir o controle total do dispositivo do sharer.|
|elevation|2|Esse status indica uma sessão em que o auxiliar foi capaz de tomar ações administrativas no dispositivo do sharer.|



