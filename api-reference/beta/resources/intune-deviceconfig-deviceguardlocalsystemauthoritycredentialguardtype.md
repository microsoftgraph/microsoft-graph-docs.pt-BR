---
title: Tipo de número deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c4369a5bf5752edf9c0636f31f936ecd43048407
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817107"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>Tipo de número deviceGuardLocalSystemAuthorityCredentialGuardType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis das configurações do Credential Guard.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Desliga o Credential Guard remotamente se configurado anteriormente sem o Bloqueio UEFI.|
|enableWithUEFILock|1|A liga o Credential Guard com o bloqueio UEFI.|
|enableWithoutUEFILock|2|A liga o Credential Guard sem o bloqueio UEFI.|
|desabilitar|3|Desabilita o Credential Guard. Esse é o valor padrão do sistema operacional.|



