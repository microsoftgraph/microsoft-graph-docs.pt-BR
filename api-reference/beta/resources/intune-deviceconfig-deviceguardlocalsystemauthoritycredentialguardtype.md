---
title: tipo de enumeração deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fe99f1896a58839d40becc6e899bab2c69e59f46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985955"
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






