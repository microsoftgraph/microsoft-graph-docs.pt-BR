---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fda734d6d582f8b838e0dca26ae57c118f3438b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526829"
---
# <a name="defenderthreataction-enum-type"></a>tipo de enumeração defenderThreatAction

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação padrão do defender a ser executada em ameaças de malware detectadas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Aplicar ação com base na definição de atualização.|
|ordena|1 |Limpe a ameaça detectada.|
|quarentena|2 |Colocar em quarentena a ameaça detectada.|
|remover|3 |Remova a ameaça detectada.|
|permitiu|4 |Permitir a ameaça detectada.|
|UserDefined|5 |Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.|
|Larga|6 |Bloquear a ameaça detectada.|



