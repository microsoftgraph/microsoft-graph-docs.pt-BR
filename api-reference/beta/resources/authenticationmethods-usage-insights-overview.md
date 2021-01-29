---
title: Trabalhando com a API do relatório de uso dos métodos de autenticação
description: O relatório de uso de métodos de autenticação ajuda uma organização a entender como seus usuários finais estão usando os recursos do Azure Active Directory, como redefinição de senha de autoatendado e autenticação multifato (MFA).
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: ba46366db81c2fbd754e7e7b83769af65b078294
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052486"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>Trabalhando com a API do relatório de uso dos métodos de autenticação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os relatórios de uso dos métodos de autenticação ajudam a entender como os usuários em sua organização usam os recursos do Azure Active Directory (Azure AD), como a Autenticação Multifatofa (MFA), Self-Service Redefinição de Senha (SSPR) e autenticação sem senha.

Esses relatórios fornecem informações como:

- Quantos usuários estão registrados para cada método de autenticação
- Quantos usuários estão registrados para recursos como Autenticação Multifatória (MFA), Self-Service Redefinição de Senha (SSPR) e autenticação sem senha.
- As taxas de falha de cada método de autenticação 

## <a name="permissions"></a>Permissões
As permissões a seguir são necessárias para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Reports.Read.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

Para acessar a API, [uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) é necessária:

* Leitor de relatórios
* Leitor de segurança
* Administrador de segurança
* Leitor global
* Administração global

## <a name="licenses"></a>Licenças

Uma licença P1 ou P2 do Azure AD Premium é necessária para acessar o uso e as informações. As informações de licenciamento da Autenticação Multifa factor do Azure AD e da redefinição de senha de autoatendado (SSPR) podem ser encontradas no site de preços do [Azure Active Directory.](https://azure.microsoft.com/pricing/details/active-directory/)

## <a name="common-requests"></a>Solicitações comuns

A tabela a seguir lista algumas solicitações comuns que você pode usar com essa API.

| Operação | Experimente o Explorador do Graph | Descrição |
| --------- | --- | ----------- |
| [getCredentialUserRegistrationcount](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | Obter o número de usuários registrados para redefinição de senha de autoatendado e MFA. |
| [getCredentialUsageSummary](/graph/api/resources/credentialusagesummary?view=graph-rest-beta&preserve-view=true) | [GET /credentialusagesummary](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | Obter o número de usuários que usam a redefinição de senha de autoatendado. |
| [credentialUserRegistrationDetails](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationdetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | Obter os detalhes do usuário para redefinição de senha de autoatendado e atividades de registro da MFA. |
| [userCredentialUsageDetails](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta&preserve-view=true) | [GET /usercredentialusagedetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | Obter detalhes do usuário para todas as atividades de redefinição de senha de autoatendado. |
| [usersRegisteredByFeature](/graph/api/resources/userregistrationfeaturesummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta) | Obter o número de usuários capazes de autenticação multifa factor, redefinição de senha de autoatendado e autenticação sem senha. |
| [usersRegisteredByMethod](/graph/api/resources/userregistrationmethodsummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta) | Obter o número de usuários registrados para cada método de autenticação. |

## <a name="next-steps"></a>Próximas etapas

- Saiba como implantar [a redefinição de senha self-service do Azure Active Directory.](/azure/active-directory/authentication/howto-sspr-deployment)
- Saiba como implantar a [MFA do Azure Active Directory.](/azure/active-directory/authentication/howto-mfa-getstarted)
- Saiba como habilitar o [registro combinado de informações de segurança.](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)