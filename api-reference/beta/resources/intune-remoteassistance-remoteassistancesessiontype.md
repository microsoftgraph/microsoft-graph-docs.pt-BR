---
title: Tipo denum remoteAssistanceSessionType
description: 'Tipo da sessão de assistência remota realizada. Os valores possíveis são: `viewOnly` , `fullControl`'
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb9f988c566c8a6e6bfc44f228d23fee8b20a1a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039466"
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



