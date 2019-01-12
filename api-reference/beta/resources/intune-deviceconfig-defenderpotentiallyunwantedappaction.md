---
title: tipo de enum defenderPotentiallyUnwantedAppAction
description: Ação do Defender executar em detectadas aplicativo potencialmente indesejadas (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 96a3dd70ae0f56f2d0d5a9d6c4f87846e10bba45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938556"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>tipo de enum defenderPotentiallyUnwantedAppAction

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ação do Defender executar em detectadas aplicativo potencialmente indesejadas (PUA).
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Proteção de PUA está desativado. Defender não protegerá contra aplicativos potencialmente indesejados.|
|bloquear|1|Proteção de PUA é no. Itens detectados serão bloqueados. Eles serão exibidas no histórico junto com outras ameaças.|
|auditoria|2|Modo de auditoria. Defender detectar aplicativos potencialmente indesejados, mas não execute nenhuma ações. Você pode revisar as informações sobre aplicativos Defender teria levado ação contra pesquisando criados pelo Defender no evento Visualizador de eventos.|





