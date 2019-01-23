---
title: tipo de enum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397453"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>tipo de enum lanManagerAuthenticationLevel

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Valores possíveis para LanManagerAuthenticationLevel

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|lmAndNltm|0|Enviar LM & respostas NTLM|
|lmNtlmAndNtlmV2|1|Enviar a segurança da sessão do LM & usar NTLM NTLMv2 se negociado|
|lmAndNtlmOnly|2|Enviar LM & somente respostas NTLM|
|lmAndNtlmV2|3|Enviar LM & respostas NTLMv2|
|lmNtlmV2AndNotLm|4|Envie LM & respostas NTLMv2. Recusar LM|
|lmNtlmV2AndNotLmOrNtm|5|Envie LM & respostas NTLMv2. Recusar LM e NTLM &|




