---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ad3ff24cc902a943fd9c146310d58cd1f1bfbd8d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088116"
---
# <a name="vpnauthenticationmethod-enum-type"></a>tipo de enumeração vpnAuthenticationMethod

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Método de autenticação VPN.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|certificado|,0|Autenticar com um certificado.|
|usernameAndPassword|1|Usar nome de usuário e senha para autenticação.|
|sharedSecret|duas|Usar segredo compartilhado para autenticação.  Válido somente para iOS IKEv2.|
|derivedCredential|3D|Use a credencial derivada para autenticação.|



