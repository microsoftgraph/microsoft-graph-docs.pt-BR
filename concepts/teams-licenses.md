---
title: Requisitos de licenciamento e pagamento
description: Saiba mais sobre os modelos de licenciamento e pagamento que se aplicam às APIs do Microsoft Teams no Microsoft Graph.
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: e3f8637bc55c6cd1cb9055d6b914063b8980e858
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262103"
---
# <a name="licensing-and-payment-requirements-for-microsoft-teams-apis-in-microsoft-graph"></a>Requisitos de licenciamento e pagamento para APIs do Microsoft Teams no Microsoft Graph

Este artigo descreve os requisitos de licenciamento e pagamento para APIs do Microsoft Teams.

Algumas APIs oferecem a opção de escolher um modelo de licenciamento e pagamento por meio do parâmetro de consulta `model`; outras suportam somente um modelo ou não suportam um modelo de licenciamento e pagamento. Os seguintes modelos de licenciamento estão disponível:

- [`model=A`](#modela-requirements) é restrito a aplicativos que executam uma [função de segurança ou conformidade](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms) e exige uma [licença com suporte.](#required-licenses-for-modela)
No futuro, os aplicativos também serão obrigados a pagar pelas mensagens que consomem além da [capacidade de propagação](#seeded-capacity).

- [`model=B`](#modelb-requirements) é restrito a aplicações que não desempenham uma [função de segurança ou de conformidade](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms). 
[`model=B`](#modelb-requirements) está livre para usar hoje; no entanto, no futuro, os aplicativos pagarão com base no número de mensagens que consomem. Não há requisitos de licenciamento para `model=B`.

- [O Modo de Avaliação (padrão)](#evaluation-mode-default-requirements) permite o acesso a APIs com uso limitado por aplicativo solicitando para fins de avaliação. As notificações de alteração não serão enviadas se o limite for excedido.

## <a name="modela-requirements"></a>Requisitos do `model=A`

`model=A` é restrito a aplicativos que executam uma função de segurança ou conformidade. Para obter detalhes, consulte a seção Termos da API para Aplicativos de Segurança e Conformidade dos [termos do produto para Serviços do Microsoft Azure](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms).

|API                   | Quem precisa de uma [licença](#required-licenses-for-modela)  | Capacidade propagada | [Preço para uso adicional](#price-for-additional-use) | Notas |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [notificações de alteração do chatMessage](/graph/api/subscription-post-subscriptions) | Remetente de mensagem | 800 mensagens por usuário por mês por aplicativo | $0,00075 por mensagem | A capacidade de semente é compartilhada com notificações de alteração de conversationMember |
| [notificações de alteração de conversationMember](/graph/api/subscription-post-subscriptions) | Qualquer usuário no locatário | 800 notificações por usuário por mês por aplicativo  | US$ 0,00075 por notificação | A capacidade de propagação é compartilhada com notificações de alteração do chatMessage |
| [Obter mensagens em todos os chats para o usuário](/graph/api/chats-getallmessages) | Usuário nomeado | 1600 mensagens por usuário por mês por aplicativo | $0,00075 por mensagem | O usuário nomeado é o usuário identificado na URL de solicitação GET. Cobrança mínima de 1 mensagem por solicitação de API. A capacidade de propagação é compartilhada com a exportação de canal. |
|  [Obtenha todas as mensagens em todos os canais](/graph/api/channel-getallmessages).| Qualquer membro da equipe | 1600 mensagens por usuário por mês por aplicativo | $0,00075 por mensagem |  Cobrança mínima de 1 mensagem por solicitação de API. A capacidade de propagação é compartilhada com a exportação de chat. |
| [Atualizando a policyViolation do chatMessage](/graph/api/chatmessage-update) |  Remetente de mensagem |  800 mensagens por usuário por mês por aplicativo | $0,00075 por mensagem |

## <a name="modelb-requirements"></a>Requisitos do `model=B`

`model=B` é restrito a aplicações que não desempenham uma função de segurança ou de conformidade. Para obter detalhes, consulte a seção Termos da API para Aplicativos de Segurança e Conformidade dos [termos do produto para Serviços do Microsoft Azure](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftAzure/MCA#ServiceSpecificTerms).

>**Observação:**[`model=B`](#modelb-requirements) é gratuito para uso hoje; no entanto, no futuro, os aplicativos pagarão com base no número de mensagens que consumirem. 

|API                   | Quem precisa de uma [licença](#required-licenses-for-modela)  | Capacidade propagada | [Preço para uso adicional](#price-for-additional-use) | Notas |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [notificações de alteração do chatMessage](/graph/api/subscription-post-subscriptions) | N/D | Nenhum | $0,00075 por mensagem |  |
| [notificações de alteração de conversationMember](/graph/api/subscription-post-subscriptions) | N/D | Nenhum  | US$ 0,00075 por notificação | |
| [Obter mensagens em todos os chats para o usuário](/graph/api/chats-getallmessages) |  N/D | Nenhum | $0,00075 por mensagem |  Cobrança mínima de 1 mensagem por solicitação de API. |
|  [Obtenha todas as mensagens em todos os canais](/graph/api/channel-getallmessages).|  N/D | Nenhum | $0,00075 por mensagem | Cobrança mínima de 1 mensagem por solicitação de API. |

## <a name="evaluation-mode-default-requirements"></a>Requisitos do modo de avaliação (padrão)

|API                   | Quem precisa de uma [licença](#required-licenses-for-modela)  | Capacidade propagada | [Preço para uso adicional](#price-for-additional-use) | Notas |
|:-----------------------------|:--------------------------------------------|:----------------|:-------|:------|
| [notificações de alteração do chatMessage](/graph/api/subscription-post-subscriptions) |  N/D | 500 mensagens por mês por aplicativo | N/D |
| [notificações de alteração de conversationMember](/graph/api/subscription-post-subscriptions) | N/D | 500 mensagens por mês por aplicativo | N/D | 
| [Obter mensagens em todos os chats para o usuário](/graph/api/chats-getallmessages) |  N/D | 500 mensagens por mês por aplicativo | N/D |  Cobrança mínima de 1 mensagem por solicitação de API. |
|  [Obtenha todas as mensagens em todos os canais](/graph/api/channel-getallmessages).|  N/D | 500 mensagens por mês por aplicativo | N/D |  Cobrança mínima de 1 mensagem por solicitação de API. |
| [Atualizando a policyViolation do chatMessage](/graph/api/chatmessage-update) |   N/D |  500 mensagens por mês por aplicativo | N/D |

No modo de avaliação, a capacidade de propagação é compartilhada em todas as APIs. Quando a capacidade de propagação for excedida, as chamadas de API com requisitos de licenciamento e pagamento falharão com um código de erro 402, e as assinaturas com requisitos de licenciamento e pagamento não enviarão notificações de alteração.

> **Observação**: uma chamada de API bem-sucedida não significa que o licenciamento adequado está no local. 
> Nem todas as violações de licença podem ser detectadas, e os períodos de carência podem ser concedidos em alguns casos.

## <a name="required-licenses-for-modela"></a>Licenças necessárias para `model=A` 

O usuário precisará de uma das [licenças com suporte.](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#microsoft-graph-apis-for-teams-data-loss-prevention-dlp-and-for-teams-export) Qual usuário precisa da licença varia de acordo com a API; para obter detalhes, consulte os [`model=A` requisitos](#modela-requirements).

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

> **Observação**: uma chamada de API bem-sucedida não significa que o licenciamento adequado está no local. 
> Nem todas as violações de licença podem ser detectadas, e os períodos de carência podem ser concedidos em alguns casos.
> Da mesma forma, o sucesso da API no modo de avaliação não garante que a chamada está dentro da capacidade semeada, pois os períodos de carência podem ser concedidos em alguns casos.

## <a name="seeded-capacity"></a>Capacidade propagada

A capacidade de propagação é a quantidade de capacidade que um aplicativo pode usar antes que um medidor de consumo seja cobrado.
A capacidade é acumulada no nível do locatário - a capacidade de propagação para todos os usuários no locatário é adicionada e comparada com o uso do aplicativo no locatário.
A capacidade de propagação é por aplicativo por locatário. Os aplicativos não ficarão sem capacidade de propagação se outro aplicativo se esgotar.

A capacidade de propagação difere pela API, consulte [ `model=A` requisitos](#modela-requirements) e [ `model=B` requisitos](#modelb-requirements)

## <a name="price-for-additional-use"></a>Preço para uso adicional

No futuro, a Microsoft cobrará uma taxa de uso sobre a capacidade de propagação. Você também será capaz associar uma assinatura do Azure ao registro de aplicativo.
