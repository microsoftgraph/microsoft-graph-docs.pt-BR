---
title: Visão geral das credenciais de identidade federada no Azure Active Directory (visualização)
description: As credenciais de identidade federada permitem que você acesse recursos do Azure e do Microsoft Graph sem ter que gerenciar segredos. Isso faz parte da federação de identidade da carga de trabalho no Azure AD.
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: conceptualPageType
ms.openlocfilehash: 58ad41d9d0277eabf39c2e830fb15f302f3813be
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697174"
---
# <a name="overview-of-federated-identity-credentials-in-azure-active-directory-preview"></a>Visão geral das credenciais de identidade federada no Azure Active Directory (visualização)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tradicionalmente, os desenvolvedores usam certificados ou segredos de cliente para as credenciais do aplicativo para autenticar e acessar serviços no Azure AD. Para acessar os serviços no locatário do Azure AD, os desenvolvedores tiveram que armazenar e gerenciar credenciais de aplicativo fora do Azure, introduzindo os seguintes gargalos:

+ Uma carga de manutenção para certificados e segredos.
+ O risco de vazamento de segredos.
+ Certificados expirando e interrupções de serviço devido a falha na autenticação.

**As credenciais de identidade federadas** são um novo tipo de credencial que permite a federação de identidade de carga de trabalho para cargas de trabalho de software. A federação de identidade de carga de trabalho permite que você Azure Active Directory recursos protegidos (Azure AD) sem precisar gerenciar segredos (para cenários com suporte). Você cria uma relação de confiança entre um provedor de identidade externa e um aplicativo no Azure AD configurando uma credencial de identidade federada. A credencial de identidade federada é usada para indicar qual token da IdP externa deve ser confiável pelo aplicativo. Depois que essa relação de confiança for criada, sua carga de trabalho de software poderá trocar tokens confiáveis do provedor de identidade externo para tokens de acesso de plataforma de identidade da Microsoft.  Sua carga de trabalho de software usa esse token de acesso para acessar os recursos protegidos do Azure AD aos quais a carga de trabalho foi concedida acesso. Isso elimina a carga de manutenção do gerenciamento manual de credenciais e elimina o risco de vazamento de segredos ou de ter certificados expirados. Para obter mais informações e cenários com suporte, leia sobre federação de identidade [de carga de trabalho.](/azure/active-directory/develop/workload-identity-federation)

O [recurso federatedIdentityCredential](federatedidentitycredential.md) representa a configuração de uma credencial de identidade federada por meio da API Graph Microsoft. As seguintes propriedades são os blocos de construção de credenciais de identidade federada:

+ **audiences**— lista as audiências que podem aparecer no token externo. Esse campo é obrigatório e é padrão para "api://AzureADTokenExchange". Ele diz o plataforma de identidade da Microsoft deve aceitar na declaração de aud no token de entrada. Esse valor representa o Azure AD em seu provedor de identidade externa e não tem valor fixo entre provedores de identidade - talvez seja necessário criar um novo registro de aplicativo em seu IdP para servir como audiência desse token.
+ **emissor —** a URL do provedor de identidade externa e deve corresponder à declaração `issuer` do token externo que está sendo trocado.
+ **subject**— O identificador da carga de trabalho de software externo dentro do provedor de identidade externa. Como o valor da audiência, ele não tem formato fixo, pois cada IdP usa seu próprio - às vezes um GUID, às vezes um identificador delimitado por dois pontos, às vezes cadeias de caracteres arbitrárias. O valor aqui deve corresponder à subclatura dentro do token apresentado ao Azure AD.

A combinação de **emissor e**    **assunto** deve ser exclusiva   no aplicativo.  Quando a carga de trabalho de software externo solicita plataforma de identidade da Microsoft para  trocar  o token externo por um token de acesso, os valores de emissor e assunto da credencial de identidade federada são verificados em relação às declarações e fornecidas no `issuer` token `subject` externo. Se essa verificação de validação for aprovada, plataforma de identidade da Microsoft um token de acesso à carga de trabalho de software externo.

As credenciais de identidade federadas são suportadas somente em aplicativos. No máximo 20 credenciais de identidade federadas podem ser adicionadas por objeto application.

A API de credenciais de identidade federada não está disponível em [implantações de nuvem](/graph/deployments) nacionais.

## <a name="see-also"></a>Confira também

+ [Tipo de recurso federatedIdentityCredential](federatedidentitycredential.md)
+ [Federação de identidade de carga de trabalho](/azure/active-directory/develop/workload-identity-federation)
+ [O que são identidades gerenciadas para recursos do Azure?](/azure/active-directory/managed-identities-azure-resources/overview)
<!--
Future: add links to articles that use federated identity credentials to access Azure AD resources.
>
