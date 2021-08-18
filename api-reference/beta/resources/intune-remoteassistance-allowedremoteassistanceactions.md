---
title: tipo de número allowedRemoteAssistanceActions
description: Enumeração sinalizador indicando se um auxiliar pode estabelecer uma tela de exibição, tomar controle total e ação de assistência remota de elevação com um dispositivo ou um compartilhamento
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d002a27a95edc28c35dee2aeacf5e0a5a759fe5
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265488"
---
# <a name="allowedremoteassistanceactions-enum-type"></a>tipo de número allowedRemoteAssistanceActions

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Enumeração de sinalizadores indicando se um auxiliar pode estabelecer uma ação de assistência remota "Exibir tela", "Assumir controle total" e "Elevação" com um dispositivo ou sharer

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|viewScreen|1 |O auxiliar pode exibir a tela do dispositivo do sharer|
|takeFullControl|2|O auxiliar pode assumir o controle total do dispositivo do sharer|
|elevation|4 |O auxiliar pode assumir o controle total do dispositivo do sharer com privilégios elevados|




