---
title: Tipo de número defenderPotentiallyUnwantedAppAction
description: Ação do Defender para assumir o PUA (Aplicativo Potencialmente Indesejado).
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ba0d7de1c865f93edf9341288681aeff2137b632
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101664"
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



