---
title: Tipo de número vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22037a272e10c78c0d500bb20fb8955e20182170
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146559"
---
# <a name="vpnauthenticationmethod-enum-type"></a>Tipo de número vpnAuthenticationMethod

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Método de autenticação VPN.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|certificado|0|Autenticar com um certificado.|
|usernameAndPassword|1|Use nome de usuário e senha para autenticação.|
|sharedSecret|2|Use o Segredo Compartilhado para Autenticação.  Válido somente para iOS IKEv2.|
|derivedCredential|3|Use a Credencial Derivada para Autenticação.|
|azureAD|4 |Use o Azure AD para autenticação.|



