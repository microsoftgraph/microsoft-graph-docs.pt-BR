---
title: Tipo de número deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis das configurações do Credential Guard.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 23da4e368b1fa858dc9e831ac6d4b35bc7510962
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59120168"
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



