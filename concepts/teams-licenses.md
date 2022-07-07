---
title: Requisitos de licenciamento e pagamento da API do Microsoft Teams
description: 'Saiba mais sobre os modelos de licenciamento e pagamento que se aplicam à API do Microsoft Teams no Microsoft Graph: modelo=A, modelo=B e modo de avaliação.'
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 3216ecfa998cf6b2a02ec588992e8622a523038c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668157"
---
# <a name="licensing-and-payment-requirements-for-the-microsoft-teams-api"></a>Requisitos de licenciamento e pagamento para a API do Microsoft Teams

Este artigo descreve os requisitos de licenciamento e pagamento para as APIs do Microsoft Teams no Microsoft Graph.

Algumas APIs oferecem a opção de escolher um modelo de licenciamento e pagamento por meio do parâmetro de consulta `model`; outras oferecem suporte apenas a um modelo ou não dão suporte a um modelo de licenciamento e pagamento. As seguintes APIs têm cobranças de consumo:

* [Exportar conteúdo do Teams](/microsoftteams/export-teams-content)
* [Criar assinatura](/graph/api/subscription-post-subscriptions)
* [Atualizar mensagem de chat](/graph/api/chatmessage-update)
* [Obter mensagem do canal](/graph/api/chatmessage-get)
* [Receba uma mensagem no bate-papo](/graph/api/chatmessage-get)

Os seguintes modelos de licenciamento estão disponíveis:

- [`model=A`](#modela-requirements) é restrito a aplicativos que executam uma [função de segurança ou conformidade](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms) e exige uma [licença com suporte.](#required-licenses-for-modela) No futuro, os aplicativos também serão obrigados a pagar pelas mensagens que consomem além da [capacidade de propagação](#seeded-capacity).

- [`model=B`](#modelb-requirements) é restrito a aplicações que não desempenham uma [função de segurança ou de conformidade](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms).
Não há requisitos de licenciamento para `model=B`.

- [O Modo de avaliação (padrão)](#evaluation-mode-default-requirements) permite o acesso a APIs com uso limitado por aplicativo solicitando para fins de avaliação. As notificações de alteração não são enviadas se o limite for excedido.

> [!NOTE]
> A partir de 5 de julho de 2022, os eventos de preços dessas APIs atingem a disponibilidade geral. Exigimos que os aplicativos preencham este [formulário](https://aka.ms/teamsgraph/protectedApis_az) para fornecer uma assinatura ativa do Azure para fins de cobrança. Para obter detalhes, consulte as [atualizações recentes](#recent-updates-and-price-for-additional-use).

## <a name="modela-requirements"></a>Requisitos do `model=A`

`model=A` é restrito a aplicativos que executam uma função de segurança ou conformidade. Para obter detalhes, consulte a seção Termos da API para Aplicativos de Segurança e Conformidade dos [termos do produto para Serviços do Microsoft Azure](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms).

|API                   | Quem precisa de uma [licença](#required-licenses-for-modela)  | Capacidade propagada | [Preço para uso adicional](#recent-updates-and-price-for-additional-use) | Notas |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [notificações de alteração do chatMessage](/graph/api/subscription-post-subscriptions) | Remetente de mensagem | 800 mensagens por usuário por mês por aplicativo | $0,00075 por mensagem | A capacidade de semente é compartilhada com notificações de alteração de conversationMember |
| [notificações de alteração de conversationMember](/graph/api/subscription-post-subscriptions) | Qualquer usuário no locatário | 800 notificações por usuário por mês por aplicativo  | US$ 0,00075 por notificação | A capacidade de propagação é compartilhada com notificações de alteração do chatMessage |
| [Obter mensagens em todos os chats para o usuário](/graph/api/chats-getallmessages) | Usuário nomeado | 1600 mensagens por usuário por mês por aplicativo | $0,00075 por mensagem | O usuário nomeado é o usuário identificado na URL de solicitação GET. Cobrança mínima de 1 mensagem por solicitação de API. A capacidade de propagação é compartilhada com a exportação de canal. |
| [Obtenha todas as mensagens em todos os canais](/graph/api/channel-getallmessages).| Qualquer membro da equipe | 1600 mensagens por usuário por mês por aplicativo | $0,00075 por mensagem |  Cobrança mínima de 1 mensagem por solicitação de API. A capacidade de propagação é compartilhada com a exportação de chat. |
| [Atualizando a policyViolation do chatMessage](/graph/api/chatmessage-update) |  Remetente de mensagem |  800 mensagens por usuário por mês por aplicativo | $0,00075 por mensagem |

## <a name="modelb-requirements"></a>Requisitos do `model=B`

`model=B` é restrito a aplicações que não desempenham uma função de segurança ou de conformidade. Para obter detalhes, consulte a seção [Termos da API para Aplicativos de Segurança e Conformidade](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms) dos termos do produto para Serviços do Microsoft Azure.

|API                   | Quem precisa de uma [licença](#required-licenses-for-modela)  | Capacidade propagada | [Preço para uso adicional](#recent-updates-and-price-for-additional-use) | Notas |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [notificações de alteração do chatMessage](/graph/api/subscription-post-subscriptions) | N/D | Nenhum | $0,00075 por mensagem |  |
| [notificações de alteração de conversationMember](/graph/api/subscription-post-subscriptions) | N/D | Nenhum  | US$ 0,00075 por notificação | |
| [Obter mensagens em todos os chats para o usuário](/graph/api/chats-getallmessages) |  N/D | Nenhum | $0,00075 por mensagem |  Cobrança mínima de 1 mensagem por solicitação de API. |
| [Obtenha todas as mensagens em todos os canais](/graph/api/channel-getallmessages).|  N/D | Nenhum | $0,00075 por mensagem | Cobrança mínima de 1 mensagem por solicitação de API. |

## <a name="evaluation-mode-default-requirements"></a>Requisitos do modo de avaliação (padrão)

|API   | Quem precisa de uma [licença](#required-licenses-for-modela)  | Capacidade propagada | [Preço para uso adicional](#recent-updates-and-price-for-additional-use) | Notas |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [notificações de alteração do chatMessage](/graph/api/subscription-post-subscriptions) |  N/D | 500 mensagens por mês por aplicativo | N/D |
| [notificações de alteração de conversationMember](/graph/api/subscription-post-subscriptions) | N/D | 500 mensagens por mês por aplicativo | N/D | 
| [Obter mensagens em todos os chats para o usuário](/graph/api/chats-getallmessages) |  N/D | 500 mensagens por mês por aplicativo | N/D |  Cobrança mínima de 1 mensagem por solicitação de API. |
| [Obtenha todas as mensagens em todos os canais](/graph/api/channel-getallmessages).|  N/D | 500 mensagens por mês por aplicativo | N/D |  Cobrança mínima de 1 mensagem por solicitação de API. |
| [Atualizando a policyViolation do chatMessage](/graph/api/chatmessage-update) |   N/D |  500 mensagens por mês por aplicativo | N/D |

No modo de avaliação, a capacidade de propagação é compartilhada em todas as APIs. Quando a capacidade de propagação for excedida, as chamadas de API com requisitos de licenciamento e pagamento falharão com um código de erro 402, e as assinaturas com requisitos de licenciamento e pagamento não enviarão notificações de alteração.

## <a name="required-licenses-for-modela"></a>Licenças necessárias para `model=A` 

O usuário precisará de uma licença que suporte o [plano de serviço](/azure/active-directory/enterprise-users/licensing-service-plan-reference) DLP de Comunicações da Microsoft, como uma dessas [licenças suportadas](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#microsoft-graph-apis-for-teams-data-loss-prevention-dlp-and-for-teams-export).
Qual usuário precisa da licença varia de acordo com a API; para obter detalhes, consulte os [`model=A` requisitos](#modela-requirements).

Os usuários convidados estão isentos desses requisitos de licenciamento.
Da mesma forma, as mensagens enviadas de fora do locatário (chat federado) são isentas.
Os medidores de consumo ainda se aplicam.

É responsabilidade do proprietário do locatário (não o proprietário do aplicativo) garantir que os usuários sejam licenciados corretamente.
Os administradores podem usar o relatório de licença de proteção de informações no [Centro de Administração do Microsoft Teams](https://admin.teams.microsoft.com/analytics/reports) para ver quais usuários não têm uma licença com suporte.

Muitas licenças com suporte oferecem avaliação gratuita. 
[Office 365 E5](https://www.microsoft.com/microsoft-365/enterprise/office-365-e5?activetab=pivot%3aoverviewtab) por exemplo tem `Free trial` um link abaixo do botão `Buy`.

Você pode obter uma assinatura de área restrita do Microsoft 365 E5 para desenvolvedores gratuita com 25 licenças de usuário por meio do [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).

## <a name="improper-licensing-and-evaluation-mode-seeded-capacity-exceeded"></a>Capacidade de propagação de licenciamento e avaliação inadequada excedida

Caso o licenciamento inadequado seja detectado, a chamada da API falhará e os dados não serão retornados.
Especificamente, para a maioria das APIs, a tentativa de OBTER mensagens para um usuário não aprovado resultará em um código de erro 402. Para notificações de alteração, as mensagens enviadas por usuários não licenciados não gerarão uma notificação de alteração. Da mesma forma, as chamadas de API e as notificações de alteração usadas no modo de avaliação em excesso da capacidade de propagação falharão.

| Tipo de erro de exemplo | Código de status | Mensagem de erro de exemplo |
|:-----------|:-----------|:-----------------|
|Requisito de licença E5 não atendido| 402 (Pagamento Obrigatório) |`...needs a valid license to access this API...`, `...tenant needs a valid license to access this API...`|
|Não há suporte para o modelo B na API de Patch| 402 (Pagamento Obrigatório) |`...query parameter 'model' does not support value 'B' for this API. Use billing model 'A'...`|
|Capacidade de avaliação excedida|402 (Pagamento Obrigatório)|`...evaluation mode capacity has been exceeded. Use a valid billing model...`|


> [!NOTE]
> Uma chamada de API bem-sucedida não significa que o licenciamento adequado está no local. Da mesma forma, o sucesso da API no modo de avaliação não garante que a chamada esteja dentro da capacidade propagada.

## <a name="seeded-capacity"></a>Capacidade propagada

A capacidade de propagação é a quantidade de capacidade que um aplicativo pode usar antes que um medidor de consumo seja cobrado. A capacidade é acumulada no nível do locatário&mdash;a capacidade de propagação para todos os usuários no locatário é adicionada e comparada com o uso do aplicativo no locatário. A capacidade de propagação é por aplicativo por locatário&mdash;os aplicativos não ficarão sem capacidade de propagação se outro aplicativo se esgotar.

A capacidade de propagação difere pela API; veja os [`model=A` requisitos](#modela-requirements) e [`model=B` requisitos](#modelb-requirements).

## <a name="recent-updates-and-price-for-additional-use"></a>Atualizações recentes e preço para uso adicional

Em outubro de 2021 [,](https://devblogs.microsoft.com/microsoft365dev/announcing-general-availability-of-microsoft-graph-export-api-for-microsoft-teams-messages/#license-requirements-for-microsoft-graph-api-for-teams-export-and-dlp) comunicamos os encargos futuros para o consumo dessas APIs; em 5 de julho de 2022, esses preços entrarão em vigor conforme  [anunciado anteriormente](https://devblogs.microsoft.com/microsoft365dev/upcoming-billing-changes-for-microsoft-graph-apis-for-teams-messages/). Se seus aplicativos estiverem ou estiverem chamando qualquer uma dessas APIs, exigimos que você preencha este [formulário de solicitação](https://aka.ms/teamsgraph/protectedApis_az) fornecendo uma assinatura ativa do Azure. Quando o [formulário](https://aka.ms/teamsgraph/protectedApis_az) tiver sido enviado para registrar um aplicativo, você poderá continuar usando essas APIs. Seguiremos as próximas etapas para integrar seu aplicativo à cobrança. 

Observe que a organização que possui o registro do aplicativo é responsável pelo pagamento e a assinatura do Azure também deve estar ativa no mesmo locatário. Para aplicativos multilocatário, a organização pode ser diferente da organização que executa o aplicativo.
