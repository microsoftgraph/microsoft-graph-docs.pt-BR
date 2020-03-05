---
title: tipo de enumeração defenderPotentiallyUnwantedAppAction
description: Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4eeadad81c86217048590cff73a212e830e1f94f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526891"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>tipo de enumeração defenderPotentiallyUnwantedAppAction

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação do defender a ser executada em aplicativo potencialmente indesejado (PUA).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|A proteção do PUA está desativada. O defender não protegerá contra aplicativos potencialmente indesejados.|
|Larga|1 |A proteção do PUA está ativada. Os itens detectados são bloqueados. Eles serão mostrados em histórico junto com outras ameaças.|
|Faça|2 |Modo de auditoria. O defender detectará aplicativos potencialmente indesejados, mas não realizará ações. Você pode revisar as informações sobre os aplicativos que o defender teria feito com a pesquisa de eventos criados pelo defender no Visualizador de eventos.|



