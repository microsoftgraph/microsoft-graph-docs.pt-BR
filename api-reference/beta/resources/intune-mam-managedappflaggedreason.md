---
title: tipo de enumeração managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 40a9d347a86df672f80ffe9b7aeda7f7f2750283
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43372928"
---
# <a name="managedappflaggedreason-enum-type"></a>tipo de enumeração managedAppFlaggedReason

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O motivo pelo qual um usuário foi sinalizado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|,0|Nenhum problema.|
|rootedDevice|1 |O registro do aplicativo está em execução em um dispositivo raiz/desbloqueado.|
|androidBootloaderUnlocked|2 |O registro do aplicativo está em execução em um dispositivo Android no qual o carregador de erro é desbloqueado.|
|androidFactoryRomModified|3 |O registro do aplicativo está em execução em um dispositivo Android em que a ROM de fábrica foi modificada.|



