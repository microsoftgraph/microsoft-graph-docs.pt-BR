---
title: Tipo de número defenderPotentiallyUnwantedAppAction
description: Ação do Defender para assumir o PUA (Aplicativo Potencialmente Indesejado).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 25bf816c93d48030cf1937669293f4cadf8e1c5f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797546"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>Tipo de número defenderPotentiallyUnwantedAppAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação do Defender para assumir o PUA (Aplicativo Potencialmente Indesejado).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|A Proteção PUA está desligada. O Defender não protegerá contra aplicativos potencialmente indesejados.|
|block|1|A Proteção pua está em. Os itens detectados são bloqueados. Eles aparecerão na história juntamente com outras ameaças.|
|audit|2|Modo de auditoria. O Defender detectará aplicativos potencialmente indesejados, mas não tomará nenhuma ação. Você pode revisar informações sobre aplicativos que o Defender teria tomado medidas em relação à pesquisa de eventos criados pelo Defender no Visualizador de Eventos.|



