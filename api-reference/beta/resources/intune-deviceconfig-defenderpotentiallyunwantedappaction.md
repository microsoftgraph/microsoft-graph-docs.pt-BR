---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente inDesejado (PUA).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1949ec58c7cfd2d896308f740b7eca16f2646b3e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800186"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>tipo de enumeração defenderPotentiallyUnwantedAppAction

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação do defender a ser executada em aplicativo potencialmente inDesejado (PUA).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|A proteção do PUA está desativada. O defender não protegerá contra aplicativos potencialmente indesejados.|
|Larga|1|A proteção do PUA está ativada. Os itens detectados são bloqueados. Eles serão mostrados em histórico junto com outras ameaças.|
|Faça|duas|Modo de auditoria. O defender detectará aplicativos potencialmente indesejados, mas não realizará ações. Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.|





