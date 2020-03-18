---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0c99cf04b217239fb1a06b2a6c26dcacc6c61cf7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794463"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>tipo de enumeração defenderPotentiallyUnwantedAppAction

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|A proteção do PUA está desativada. O defender não protegerá contra aplicativos potencialmente indesejados.|
|Larga|1|A proteção do PUA está ativada. Os itens detectados são bloqueados. Eles serão mostrados em histórico junto com outras ameaças.|
|Faça|duas|Modo de auditoria. O defender detectará aplicativos potencialmente indesejados, mas não realizará ações. Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.|



