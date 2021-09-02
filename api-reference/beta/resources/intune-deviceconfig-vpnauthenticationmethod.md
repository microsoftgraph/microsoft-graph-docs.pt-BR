---
title: Tipo de número vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 83d1789f02c8cc961bd4d1c784ad70f47c6b7f85
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789930"
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



