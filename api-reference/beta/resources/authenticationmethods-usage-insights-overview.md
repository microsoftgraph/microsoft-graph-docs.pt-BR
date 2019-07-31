---
title: Trabalhar com a API de relatório de uso dos métodos de autenticação
description: O relatório de uso dos métodos de autenticação ajuda uma organização a entender como os usuários finais estão usando recursos do Azure Active Directory, como redefinição de senha de autoatendimento e autenticação multifator (MFA).
author: davidmu1
localization_priority: Normal
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 4f8886333d5067abc42a583084726c58ec67a659
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013196"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>Trabalhar com a API de relatório de uso dos métodos de autenticação

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os relatórios de uso dos métodos de autenticação ajudam você a compreender como os usuários da sua organização usam os recursos do Azure Active Directory (Azure AD), como a senha de autoatendimento e a autenticação multifator (MFA).

Esses relatórios fornecem informações como:

- Quais métodos de autenticação são mais bem sucedidos para sua organização. 
- Quais tipos de erros os usuários finais estão executando.
- Qual campanha você precisa executar para ajudar os usuários finais a adotar o uso da senha de autoatendimento REST e da MFA.

## <a name="common-requests"></a>Solicitações comuns

A tabela a seguir lista algumas solicitações comuns que você pode usar com essa API.

| Operation | Experimente o Explorador do Graph | Descrição |
| --------- | --- | ----------- |
| [getCredentialUserRegistrationcount](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta) | [OBTER/credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | Obtenha o número de usuários registrados para redefinição e MFA de senha de autoatendimento. |
| [getCredentialUsageSummary](/graph/api/resources/credentialusagesummary?view=graph-rest-beta) | [OBTER/credentialusagesummary](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | Obtenha o número de usuários usando a redefinição de senha de autoatendimento. |
| [credentialUserRegistrationDetails](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) | [OBTER/credentialuserregistrationdetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | Obtenha os detalhes do usuário para as atividades de redefinição de senha de autoatendimento e de registro de MFA. |
| [userCredentialUsageDetails](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) | [OBTER/usercredentialusagedetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | Obtenha detalhes do usuário para todas as atividades de redefinição de senha de autoatendimento. |

## <a name="licenses"></a>Licenças

Relatórios de uso estão disponíveis para recursos licenciados que aproveitam a redefinição de senha de autoatendimento e a MFA em seu locatário.

## <a name="next-steps"></a>Próximas etapas

- Saiba como implantar a redefinição de [senha de autoatendimento do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).
- Saiba como implantar o [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).
- Saiba como habilitar o [registro de informações de segurança combinado](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).



