---
title: Visão geral das credenciais de identidade federada no Azure Active Directory (visualização)
description: As credenciais de identidade federada permitem que você acesse recursos do Azure e do Microsoft Graph sem ter que gerenciar segredos. Isso faz parte da federação de identidade da carga de trabalho no Azure AD.
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: conceptualPageType
ms.openlocfilehash: ab3bfbd94ef77b7e7dd2c0a9e4a156806ab47c11
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804000"
---
# <a name="overview-of-federated-identity-credentials-in-azure-active-directory-preview"></a>Visão geral das credenciais de identidade federada no Azure Active Directory (visualização)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tradicionalmente, os desenvolvedores usam certificados ou segredos de cliente para as credenciais do aplicativo para autenticar e acessar serviços no Azure AD. Para acessar os serviços no locatário do Azure AD, os desenvolvedores tiveram que armazenar e gerenciar credenciais de aplicativo fora do Azure, introduzindo os seguintes gargalos:

+ Uma carga de manutenção para certificados e segredos.
+ O risco de vazamento de segredos.
+ Certificados expirando e interrupções de serviço devido a falha na autenticação.

**As credenciais de identidade federadas** são um novo tipo de credencial que permite a federação de identidade de carga de trabalho para cargas de trabalho de software. A federação de identidade de carga de trabalho permite que você Azure Active Directory recursos protegidos (Azure AD) sem precisar gerenciar segredos (para cenários com suporte).

## <a name="how-do-federated-identity-credentials-work"></a>Como funcionam as credenciais de identidade federada?

Você cria uma relação de confiança entre um provedor de identidade externa (IdP) e um aplicativo no Azure AD configurando uma credencial de identidade federada. A credencial de identidade federada é usada para indicar qual token da IdP externa deve ser confiável pelo aplicativo. Depois que essa relação de confiança for criada, sua carga de trabalho de software poderá trocar tokens confiáveis do provedor de identidade externo para tokens de acesso do plataforma de identidade da Microsoft. Sua carga de trabalho de software usa esse token de acesso para acessar os recursos protegidos do Azure AD aos quais a carga de trabalho foi concedida acesso. Isso elimina a carga de manutenção do gerenciamento manual de credenciais e elimina o risco de vazamento de segredos ou de ter certificados expirados. Para obter mais informações e cenários com suporte, consulte [federação de identidade de carga de trabalho](/azure/active-directory/develop/workload-identity-federation).

## <a name="set-up-federated-identity-credentials-through-microsoft-graph"></a>Configurar credenciais de identidade federada por meio do Microsoft Graph

O [recurso federatedIdentityCredential](federatedidentitycredential.md) representa a configuração de uma credencial de identidade federada por meio do Microsoft Graph. As seguintes propriedades são os blocos de construção de credenciais de identidade federada:

+ **audiências** — lista as audiências que podem aparecer no token externo. Esse campo é obrigatório e o padrão é `api://AzureADTokenExchange`. Ele diz o plataforma de identidade da Microsoft deve aceitar na declaração de aud no token de entrada. Esse valor representa o Azure AD em seu provedor de identidade externa e não tem valor fixo entre provedores de identidade - talvez seja necessário criar um novo registro de aplicativo em seu IdP para servir como audiência desse token.
+ **emissor —** a URL do provedor de identidade externa. Deve corresponder **à declaração do emissor** do token externo que está sendo trocado.
+ **subject** — O identificador da carga de trabalho de software externo dentro do provedor de identidade externa. Como o valor da audiência, ele não tem formato fixo, pois cada IdP usa seu próprio - às vezes um GUID, às vezes um identificador delimitado por dois pontos, às vezes cadeias de caracteres arbitrárias. O valor aqui deve corresponder à subclatura dentro do token apresentado ao Azure AD.

A combinação  **ofissuerandsubject**   **deve**  ser exclusiva no aplicativo.  Quando a carga de trabalho de software externo solicita plataforma de identidade da Microsoft para trocar o token externo por um token de acesso,  os valores de  emissor e assunto da credencial de identidade federada `issuer` `subject` são verificados em relação às declarações e fornecidas no token externo. Se essa verificação de validação for aprovada, plataforma de identidade da Microsoft um token de acesso à carga de trabalho de software externo.

A API de credenciais de identidade federada não está disponível em [implantações de nuvem](/graph/deployments) nacionais.

## <a name="design-considerations"></a>Considerações de design

As credenciais de identidade federadas são suportadas somente em aplicativos. No máximo 20 credenciais de identidade federadas podem ser adicionadas por objeto application.

## <a name="see-also"></a>Confira também

+ [Tipo de recurso federatedIdentityCredential](federatedidentitycredential.md)
+ [Federação de identidade de carga de trabalho](/azure/active-directory/develop/workload-identity-federation)
+ [O que são identidades gerenciadas para recursos do Azure?](/azure/active-directory/managed-identities-azure-resources/overview)
<!--
Future: add links to articles that use federated identity credentials to access Azure AD resources.
>
