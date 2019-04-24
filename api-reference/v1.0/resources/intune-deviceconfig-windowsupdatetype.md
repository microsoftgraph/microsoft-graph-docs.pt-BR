---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f91657cabec59cf1307253d707ba632bf4f99463
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503594"
---
# <a name="windowsupdatetype-enum-type"></a>tipo de enumeração windowsUpdateType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Para quais dispositivos de filial receberão suas atualizações

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|,0|Permite que o usuário defina.|
|todos os|1 |Canal semestral (direcionado). O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).|
|businessReadyOnly|2 |Canal semestral. O dispositivo Obtém atualizações de recursos do canal semestral.|
|windowsInsiderBuildFast|3 |Compilação do Windows inSider-Fast|
|windowsInsiderBuildSlow|4 |Compilação do Windows inSider-lenta|
|windowsInsiderBuildRelease|5 |Versão de lançamento do Windows inSider|



