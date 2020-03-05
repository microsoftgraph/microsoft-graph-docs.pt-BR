---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 94c82e45aae328f35b890f82755609945a9b58f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528924"
---
# <a name="windowsupdatetype-enum-type"></a>tipo de enumeração windowsUpdateType

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Para quais dispositivos de filial receberão suas atualizações

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|todos os|1 |Canal semestral (direcionado). O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).|
|businessReadyOnly|2 |Canal semestral. O dispositivo Obtém atualizações de recursos do canal semestral.|
|windowsInsiderBuildFast|3 |Compilação do Windows Insider-Fast|
|windowsInsiderBuildSlow|4 |Compilação do Windows Insider-lenta|
|windowsInsiderBuildRelease|5 |Versão de lançamento do Windows Insider|



