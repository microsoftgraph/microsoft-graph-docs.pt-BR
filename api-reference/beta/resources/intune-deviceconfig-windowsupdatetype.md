---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 35fe62ada736a0cd5c3a073e49851b6cad9320ab
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786148"
---
# <a name="windowsupdatetype-enum-type"></a>tipo de enumeração windowsUpdateType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Para quais dispositivos de filial receberão suas atualizações

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|todos os|1|Canal semestral (direcionado). O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).|
|businessReadyOnly|duas|Canal semestral. O dispositivo Obtém atualizações de recursos do canal semestral.|
|windowsInsiderBuildFast|3D|Compilação do Windows Insider-Fast|
|windowsInsiderBuildSlow|4 |Compilação do Windows Insider-lenta|
|windowsInsiderBuildRelease|5 |Versão de lançamento do Windows Insider|



