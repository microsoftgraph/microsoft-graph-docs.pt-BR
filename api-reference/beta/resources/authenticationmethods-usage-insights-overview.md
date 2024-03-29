---
title: Trabalhando com a API de relatório de uso de métodos de autenticação
description: O relatório de uso dos métodos de autenticação ajuda uma organização a entender como seus usuários finais estão usando Azure Active Directory recursos como redefinição de senha de autoatendados e autenticação multifato (MFA).
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 6af5d1805b09add23cfc6c36c7d10acc1e31dc75
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201600"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>Trabalhando com a API de relatório de uso de métodos de autenticação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os relatórios de uso dos métodos de autenticação ajudam você a entender como os usuários em sua organização usam recursos do Azure Active Directory (Azure AD), como Autenticação multifatofatória (MFA), Self-Service Redefinição de Senha (SSPR) e autenticação sem senha.

Esses relatórios fornecem informações como:

- Quantos usuários são registrados para cada método de autenticação
- Quantos usuários estão registrados para recursos como Autenticação Multifafação (MFA), Self-Service Redefinição de Senha (SSPR) e autenticação sem senha.
- As taxas de falha de cada método de autenticação 

## <a name="permissions"></a>Permissões
As seguintes permissões são obrigatórias para chamar esta API. Para saber mais, incluindo como escolher as permissões, consulte [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Reports.Read.All, AuditLog.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Reports.Read.All, AuditLog.Read.All|

Para acessar a API, uma [das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) é necessária:

* Leitor de relatórios
* Leitor de segurança
* Administrador de segurança
* Leitor global
* Administração global

## <a name="licenses"></a>Licenças

Uma Azure AD Premium P1 ou P2 é necessária para acessar o uso e as percepções. As informações de licenciamento de autenticação multifafação e de redefinição de senha de autoatendificação do Azure AD (SSPR) podem ser encontradas no site Azure Active Directory [preço.](https://azure.microsoft.com/pricing/details/active-directory/)

## <a name="common-requests"></a>Solicitações comuns

A tabela a seguir lista algumas solicitações comuns que você pode usar com essa API.

| Operação | Experimente o Explorador do Graph | Descrição |
| --------- | --- | ----------- |
| [getCredentialUserRegistrationcount](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | Obter o número de usuários registrados para redefinição de senha de autoatendados e MFA. |
| [getCredentialUsageSummary](/graph/api/resources/credentialusagesummary?view=graph-rest-beta&preserve-view=true) | [GET /credentialusagesummary](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | Obter o número de usuários que usam redefinição de senha de autoatendados. |
| [credentialUserRegistrationDetails](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationdetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | Obter os detalhes do usuário para redefinição de senha de autoatendados e atividades de registro MFA. |
| [userCredentialUsageDetails](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta&preserve-view=true) | [GET /usercredentialusagedetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | Obter detalhes do usuário para todas as atividades de redefinição de senha de autoatendados. |
| [usersRegisteredByFeature](/graph/api/resources/userregistrationfeaturesummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta) | Obter o número de usuários capazes de autenticação multifafa, redefinição de senha de autoatendados e autenticação sem senha. |
| [usersRegisteredByMethod](/graph/api/resources/userregistrationmethodsummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta) | Obter o número de usuários registrados para cada método de autenticação. |
| [userRegistrationDetails](/graph/api/resources/userRegistrationDetails?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/userRegistrationDetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/userRegistrationDetails&version=beta) | Obter os detalhes do registro MFA para todos os usuários. |

## <a name="next-steps"></a>Próximas etapas

- Saiba como implantar Azure Active Directory [redefinição de senha de autoatendados.](/azure/active-directory/authentication/howto-sspr-deployment)
- Saiba como implantar o [Azure Active Directory MFA](/azure/active-directory/authentication/howto-mfa-getstarted).
- Saiba como habilitar [o registro combinado de informações de segurança.](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)
