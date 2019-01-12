---
title: tipo de enum folderProtectionType
description: Valores possíveis de proteção de pasta
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 427bdb4fcb93a831ab120aa0c7eefcbf97675fa8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973746"
---
# <a name="folderprotectiontype-enum-type"></a>tipo de enum folderProtectionType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis de proteção de pasta
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Valor de padrão de dispositivo, sem intenção.|
|Habilitar|1|Funcionalidade de bloco.|
|auditMode|2|Permitir a funcionalidade mas gerar logs.|
|blockDiskModification|3|Bloquear aplicativos não confiáveis gravem setores do disco.|
|auditDiskModification|4|Gere logs quando aplicativos não confiáveis gravar setores do disco.|





