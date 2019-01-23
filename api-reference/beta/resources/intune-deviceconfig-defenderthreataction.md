---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400267"
---
# <a name="defenderthreataction-enum-type"></a>tipo de enum defenderThreatAction

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Ação de padrão do Defender assuma detectadas ameaças de Malware.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Aplica a ação com base na definição de atualização.|
|clean|1|Limpe ameaça detectada.|
|quarentena|2|Quarentena ameaça detectada.|
|remover|3|Remova ameaça detectada.|
|permitir|4|Permitir ameaça detectada.|
|userDefined|5|Permitir que o usuário determinar a ação a ser executada com ameaça detectada.|
|bloquear|6|Bloquear ameaça detectada.|




