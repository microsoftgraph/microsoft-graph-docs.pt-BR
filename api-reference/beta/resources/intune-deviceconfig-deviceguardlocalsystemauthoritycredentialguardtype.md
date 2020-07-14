---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b02402ff6c6c0373396bd6fca0cad6ded5cb36d
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123768"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis das configurações do Credential Guard.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Desativa o Credential Guard remotamente, se configurado anteriormente sem bloqueio de UEFI.|
|enableWithUEFILock|1 |Ativa o Credential Guard com bloqueio de UEFI.|
|enableWithoutUEFILock|2 |Ativa o Credential Guard sem bloqueio de UEFI.|
|desabilitar|3 |Desabilita a proteção de credenciais. Este é o valor padrão de sistema operacional.|



