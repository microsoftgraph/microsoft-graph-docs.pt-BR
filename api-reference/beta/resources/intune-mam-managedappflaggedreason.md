---
title: Tipo de número managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 239ca0dfadd159466f9a81649b9a196f0deea332
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817044"
---
# <a name="managedappflaggedreason-enum-type"></a>Tipo de número managedAppFlaggedReason

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O motivo pelo qual um usuário foi sinalizado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Nenhum problema.|
|rootedDevice|1|O registro do aplicativo está sendo executado em um dispositivo rooted/desbloqueado.|
|androidBootloaderUnlocked|2|O registro do aplicativo está sendo executado em um dispositivo Android no qual o carregador de inicialização é desbloqueado.|
|androidFactoryRomModified|3|O registro do aplicativo está sendo executado em um dispositivo Android no qual a ROM de fábrica foi modificada.|



