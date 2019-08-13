---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 41a6d23e42d263dd8241e960af693450ac0a7c3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369504"
---
# <a name="windowsupdatetype-enum-type"></a>tipo de enumeração windowsUpdateType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Para quais dispositivos de filial receberão suas atualizações

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|todos os|1|Canal semestral (direcionado). O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).|
|businessReadyOnly|duas|Canal semestral. O dispositivo Obtém atualizações de recursos do canal semestral.|
|windowsInsiderBuildFast|3D|Compilação do Windows Insider-Fast|
|windowsInsiderBuildSlow|quatro|Compilação do Windows Insider-lenta|
|windowsInsiderBuildRelease|0,5|Versão de lançamento do Windows Insider|



