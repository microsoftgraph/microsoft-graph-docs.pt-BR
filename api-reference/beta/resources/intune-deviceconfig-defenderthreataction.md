---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bd71ee742ba7d7b5a98c5f3bbf90496bb52392be
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696262"
---
# <a name="defenderthreataction-enum-type"></a>tipo de enumeração defenderThreatAction

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação padrão do defender a ser executada em ameaças de malware detectadas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Aplicar ação com base na definição de atualização.|
|ordena|1|Limpe a ameaça detectada.|
|quarentena|duas|Colocar em quarentena a ameaça detectada.|
|remover|3D|Remova a ameaça detectada.|
|permitiu|4 |Permitir a ameaça detectada.|
|UserDefined|5 |Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.|
|Larga|6 |Bloquear a ameaça detectada.|





