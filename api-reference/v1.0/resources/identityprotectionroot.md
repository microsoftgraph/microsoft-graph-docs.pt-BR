---
title: APIs de proteção de identidade
description: tipo de recurso identityProtectionRoot
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab01fb11d7973adf056685f6ab0d6ef02e2ecb4d
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581299"
---
# <a name="identityprotectionroot-resource-type"></a>tipo de recurso identityProtectionRoot

Namespace: microsoft.graph

A proteção de identidade é uma ferramenta que permite às organizações detectar, investigar e corrigir riscos baseados em identidade em seu ambiente. Você pode usar as seguintes APIs do Microsoft Graph para consultar os riscos detectados pela proteção de identidade: 

* [riskDetection](riskdetection.md) -consulta o Microsoft Graph para obter uma lista de detecções de riscos vinculados de usuário e de entrada e informações associadas sobre a detecção. As detecções de risco na proteção de identidade do Azure AD incluem qualquer ação suspeita identificada relacionada às contas de usuário no diretório.

* [riskyUsers](riskyuser.md) – consulta o Microsoft Graph para obter informações sobre os usuários que a proteção de identidade detectou como arriscado. O risco do usuário representa a probabilidade de que uma determinada identidade ou conta seja comprometida. Esses riscos são calculados offline usando fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de imposição de leis, equipes de segurança da Microsoft e outras fontes confiáveis.

* [Sign](signin.md) -in – consultar o Microsoft Graph para obter informações sobre as entradas do Azure AD com propriedades específicas relacionadas ao estado, detalhes e nível do risco. Um risco de entrada representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade. Esses riscos podem ser calculados em tempo real ou calculados offline usando fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de imposição de leis, equipes de segurança da Microsoft e outras fontes confiáveis.

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>O que posso fazer com as APIs de proteção de identidade no Microsoft Graph?

As seguintes solicitações são populares para trabalhar com dados de log de auditoria:

Operation | URL
:----------|:----
OBTER usuários arriscados | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
OBTER detecções de risco | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
OBTER o histórico de riscos de um usuário | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
CONFIRMAR um usuário como comprometido | [Postar https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
IGNORAR um usuário arriscado | [Postar https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

## <a name="what-licenses-do-i-need"></a>De quais licenças eu preciso?

A proteção de identidade do Azure AD é um recurso Premium. Você precisa de uma licença do Azure AD Premium P1 ou P2 para acessar a API riskDetection (Observação: as licenças P1 recebem informações de risco limitado). A API riskyUsers só está disponível somente para licenças do Azure AD Premium P2.

## <a name="see-also"></a>Confira também

* [Sobre a proteção de identidade do Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection)
* [Introdução à proteção de identidade do Azure Active Directory e ao Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)