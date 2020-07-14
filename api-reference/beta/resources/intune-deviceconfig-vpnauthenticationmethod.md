---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef477b17b8ae7e8aedc3b95ce70b66115a3c8712
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123887"
---
# <a name="vpnauthenticationmethod-enum-type"></a>tipo de enumeração vpnAuthenticationMethod

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Método de autenticação VPN.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|certificado|,0|Autenticar com um certificado.|
|usernameAndPassword|1 |Usar nome de usuário e senha para autenticação.|
|sharedSecret|2 |Usar segredo compartilhado para autenticação.  Válido somente para iOS IKEv2.|
|derivedCredential|3 |Use a credencial derivada para autenticação.|
|azureAD|4 |Usar o Azure AD para autenticação.|



