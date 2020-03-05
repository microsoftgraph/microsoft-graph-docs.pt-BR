---
title: tipo de enumeração managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 64f78ca8a074d35687f50e232a104b87717a6462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527915"
---
# <a name="managedappflaggedreason-enum-type"></a>tipo de enumeração managedAppFlaggedReason

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O motivo pelo qual um usuário foi sinalizado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhuma|,0|Nenhum problema.|
|rootedDevice|1 |O registro do aplicativo está em execução em um dispositivo raiz/desbloqueado.|
|androidBootloaderUnlocked|2 |O registro do aplicativo está em execução em um dispositivo Android no qual o carregador de erro é desbloqueado.|
|androidFactoryRomModified|3 |O registro do aplicativo está em execução em um dispositivo Android em que a ROM de fábrica foi modificada.|



