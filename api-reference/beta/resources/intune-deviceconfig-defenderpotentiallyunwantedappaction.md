---
title: tipo de enum defenderPotentiallyUnwantedAppAction
description: Ação do Defender executar em detectadas aplicativo potencialmente indesejadas (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422751"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>tipo de enum defenderPotentiallyUnwantedAppAction

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Ação do Defender executar em detectadas aplicativo potencialmente indesejadas (PUA).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Proteção de PUA está desativado. Defender não protegerá contra aplicativos potencialmente indesejados.|
|bloquear|1|Proteção de PUA é no. Itens detectados serão bloqueados. Eles serão exibidas no histórico junto com outras ameaças.|
|auditoria|2|Modo de auditoria. Defender detectar aplicativos potencialmente indesejados, mas não execute nenhuma ações. Você pode revisar as informações sobre aplicativos Defender teria levado ação contra pesquisando criados pelo Defender no evento Visualizador de eventos.|




