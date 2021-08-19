---
title: Tipo de número defenderPotentiallyUnwantedAppAction
description: Ação do Defender para assumir o PUA (Aplicativo Potencialmente Indesejado).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1ef21f26b259676e774ff009eb8432d4384129fd5977bddf23daf47760742a03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54142061"
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
|block|1 |A Proteção pua está em. Os itens detectados são bloqueados. Eles aparecerão na história juntamente com outras ameaças.|
|audit|2|Modo de auditoria. O Defender detectará aplicativos potencialmente indesejados, mas não tomará nenhuma ação. Você pode revisar informações sobre aplicativos que o Defender teria tomado medidas em relação à pesquisa de eventos criados pelo Defender no Visualizador de Eventos.|




