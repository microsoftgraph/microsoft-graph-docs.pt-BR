---
title: tipo de enumeração de enrollmentid
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3002fd793020213f8787f0c62b1e7d7c1c9ee0e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523678"
---
# <a name="enrollmentstate-enum-type"></a>tipo de enumeração de enrollmentid

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado do registro do dispositivo é desconhecido|
|registrados|1 |O dispositivo está inscrito.|
|pendingReset|2 |Inscrito, mas ele está inscrito via perfil de registro e o perfil inscrito é diferente do perfil atribuído.|
|falhou|3 |Não registrado e o registro de falha de registro.|
|Não contatado|4 |O dispositivo é importado, mas não está inscrito.|
|bloqueou|5 |O dispositivo está inscrito como um não-usuário, mas é impedido de migrar para o registro do usuário porque o aplicativo não pôde ser instalado.|



