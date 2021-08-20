---
title: Tipo de número deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 84fb6ed2690218cdecdb7a277143ba76c0a804e3776981fc45beb21a2793b70a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227460"
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
|enableWithUEFILock|1 |A liga o Credential Guard com o bloqueio UEFI.|
|enableWithoutUEFILock|2|A liga o Credential Guard sem o bloqueio UEFI.|
|desabilitar|3 |Desabilita o Credential Guard. Esse é o valor padrão do sistema operacional.|




