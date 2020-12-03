---
title: Trabalhar com a API de relatório de uso dos métodos de autenticação
description: O relatório de uso dos métodos de autenticação ajuda uma organização a entender como os usuários finais estão usando recursos do Azure Active Directory, como redefinição de senha de autoatendimento e autenticação multifator (MFA).
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: fbf9bc81d37b7f102e46ae47a899403570862660
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523480"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>Trabalhar com a API de relatório de uso dos métodos de autenticação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os relatórios de uso dos métodos de autenticação ajudam a entender como os usuários da sua organização utilizam os recursos do Azure Active Directory (Azure AD), como descanso de senha de autoatendimento e autenticação multifatorial (MFA).

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

- Saiba como [implantar a redefinição de senha de autoatendimento do Azure Active Directory](/azure/active-directory/authentication/howto-sspr-deployment).
- Saiba como implantar o [Azure Active Directory MFA](/azure/active-directory/authentication/howto-mfa-getstarted).
- Saiba como habilitar o [registro de informações de segurança combinado](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).