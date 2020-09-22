---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ff44e62d67a5acde9a87e1238b72caed29677452
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089522"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>tipo de enumeração defenderPotentiallyUnwantedAppAction

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|A proteção do PUA está desativada. O defender não protegerá contra aplicativos potencialmente indesejados.|
|Larga|1 |A proteção do PUA está ativada. Os itens detectados são bloqueados. Eles serão mostrados em histórico junto com outras ameaças.|
|Faça|2 |Modo de auditoria. O defender detectará aplicativos potencialmente indesejados, mas não realizará ações. Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.|






