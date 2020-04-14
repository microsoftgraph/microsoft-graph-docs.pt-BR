---
title: tipo de enumeração de enrollmentid
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d4c3fa42d20bcf0540c55975d24aad596c8aebf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407753"
---
# <a name="enrollmentstate-enum-type"></a>tipo de enumeração de enrollmentid

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O estado do registro do dispositivo é desconhecido|
|registrados|1|O dispositivo está inscrito.|
|pendingReset|duas|Inscrito, mas ele está inscrito via perfil de registro e o perfil inscrito é diferente do perfil atribuído.|
|falhou|3D|Não registrado e o registro de falha de registro.|
|Não contatado|4 |O dispositivo é importado, mas não está inscrito.|
|bloqueou|5 |O dispositivo está inscrito como um não-usuário, mas é impedido de migrar para o registro do usuário porque o aplicativo não pôde ser instalado.|



