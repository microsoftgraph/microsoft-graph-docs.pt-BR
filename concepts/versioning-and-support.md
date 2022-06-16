---
title: Controle de versão, suporte e mudanças significativas de políticas para o Microsoft Graph
description: Saiba mais sobre o suporte e as políticas de alteração de falha do Microsoft Graph e das versões da API do Microsoft Graph que estão disponíveis no momento.
ms.localizationpriority: high
ms.openlocfilehash: 3b5b385cbf738c04b976e6ca3e0749c47942eabf
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095010"
---
# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a>Controle de versão, suporte e mudanças significativas de políticas para o Microsoft Graph

Este artigo descreve o suporte e as alterações significativas de políticas do Microsoft Graph e as versões da API Microsoft Graph disponível no momento.

## <a name="support-policy-and-deprecation-information"></a>Informações de política e substituição de suporte

O Microsoft Graph segue a [Política de Ciclo de Vida da Microsoft](https://support.microsoft.com/lifecycle).

Conforme novas versões das APIs REST Microsoft Graph e SDKs do Microsoft Graph são lançadas, as versões anteriores são desativadas. A Microsoft declara uma versão como preterida com antecedência de pelo menos 24 meses antes de preteri-la. Da mesma forma, para APIs individuais que geralmente estão disponíveis (GA), a Microsoft declara uma API como preterida com antecedência de pelo menos 24 meses antes de removê-la da versão de GA.

Quando incrementamos a versão principal da API (por exemplo, de v1.0 a v2.0), anunciamos que a versão atual (neste exemplo, v1.0) está imediatamente preterida e não haverá mais suporte para ela 24 meses após o anúncio. Podemos fazer exceções a essa política para problemas de confiabilidade de segurança ou de saúde.

Quando uma API é marcada como preterida, é altamente recomendável que você migre para a versão mais recente assim que possível. Em alguns casos, anunciaremos que os novos aplicativos deverão começar a usar as novas APIs um pouco depois das APIs originais serem preteridas. Nesses casos, apenas os aplicativos ativos que usam atualmente as APIs preteridas podem continuar a usá-las.

### <a name="api-contract-and-non-backward-compatible-changes"></a>Contrato de API e alterações sem compatibilidade com versões anteriores

O Microsoft Graph tem um log de alterações entre as versões. Essas alterações estão listadas no [Log de alterações do Microsoft Graph](changelog.md). Conforme nova funcionalidade e dados são adicionados ao Microsoft Graph, incrementaremos o número de versão da API para qualquer alteração à API não compatível com versões anteriores.

A seguir há exemplos de alterações não compatíveis com versões anteriores:

- Mudanças na URL ou solicitação/resposta fundamentais associadas ao recurso
- Remoção, renomear ou alterar o tipo de uma propriedade declarada
- Remoção ou renomeação de APIs ou parâmetros de API
- Adição de um cabeçalho de solicitação obrigatório

A seguir há exemplos de alterações compatíveis com versões anteriores:

- Adição de propriedades que são anuláveis ou têm um valor padrão
- Adição de um membro a uma enumeração
- Remover, renomear ou alterar o tipo de uma extensão aberta
- Remover, renomear ou alterar o tipo de uma anotação
- Introdução de paginação a coleções existentes
- Alterações de códigos de erro
- Alterações à ordem das propriedades
- Alterações no formato ou no comprimento de cadeias de caracteres opacas, como IDs de recurso

>**Observação:** Ao longo do tempo, atualizaremos a lista de alterações compatíveis com versões anteriores. Se você gerar seus próprios proxies de cliente (como clientes WCF), nossa orientação é que os aplicativos cliente devem estar preparados para receber propriedades e tipos derivados definidos anteriormente pelo serviço da API do Microsoft Graph. A API do Microsoft Graph segue a orientação descrita na seção [Controle de Versão de Modelo](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) nas [diretrizes da API do Microsoft REST](https://github.com/microsoft/api-guidelines/).

## <a name="versions"></a>Versões

As seguintes versões da API Microsoft Graph estão disponíveis atualmente.

### <a name="beta-version"></a>Versão beta
Em geral, as APIs são lançadas na versão beta e são acessíveis no ponto de extremidade `https://graph.microsoft.com/beta`. Para obter a documentação da API beta, veja [Referência de ponto de extremidade do Microsoft Graph beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true). Espere alterações significativas e preterimento de APIs na versão beta regularmente. Não use uma dependência de produção em APIs beta.

Não damos nenhuma garantia de que um recurso beta será promovido para a versão atual. Quando a equipe da API Microsoft Graph acreditar que um recurso beta está pronto para disponibilidade geral (GA), adicionaremos esse recurso à versão atual mais recente. Se a promoção do recurso resultar em uma alteração significativa de uma versão atual, o número da versão será incrementado e a nova versão se tornará a versão atual.
Nossa comunidade de desenvolvedores pode postar solicitações de recursos no [fórum de ideias da Plataforma para Desenvolvedores do Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph), incluindo solicitações para novos recursos, bem como solicitações para promover APIs beta existentes para a versão atual.

### <a name="current-version"></a>Versão atual

A versão atual do Microsoft Graph é a v1.0. Exposta em `https://graph.microsoft.com/v1.0`, a versão do Microsoft Graph API v1.0 contém recursos que estão geralmente disponíveis e prontos para uso de produção. Navegue pela [documentação para APIs v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=true).

## <a name="preview-status"></a>Status da visualização
Uma API ou recurso no Microsoft Graph é rotulado como "(visualização)" para indicar que seu comportamento é _exclusivo_ no ponto de extremidade beta.  

O comportamento da maioria dos recursos e das APIs na versão v1.0 está em paridade com a versão beta. "visualização" qualifica uma minoria de recursos e APIs em um dos dois casos a seguir: 
- Disponível somente em versão beta
- Disponível na versão beta de forma diferente do que no v1.0

Assim como qualquer outra API no ponto de extremidade beta, as APIs marcadas na documentação como "(visualização)" podem sofrer alterações significativas sem aviso. Não acesse as APIs do ponto de extremidade beta nos aplicativos de produção.

Como exemplo, o [treinamento de simulação de ataque](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true) é um recurso que geralmente está disponível para administradores no [portal do Microsoft 365 Defender](https://security.microsoft.com/). Quando a API REST para treinamento de simulação de ataque fica disponível no Microsoft Graph apenas no ponto de extremidade beta, a [documentação](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#attack-simulation-and-training-preview) da API REST é rotulada como "(visualização)". O rótulo "(visualização)" se aplica à API REST e sua documentação no Microsoft Graph, mesmo que o serviço em si esteja disponível para o público geral.

### <a name="deprecated-and-unsupported-versions"></a>Versões preteridas e sem suporte

Não há atualmente nenhuma versão preterida da Microsoft Graph.

## <a name="terms-of-use"></a>Termos de uso

Ao usar as APIs do Microsoft Graph, você concorda com os [Termos de Uso das APIs da Microsoft](/legal/microsoft-apis/terms-of-use?context=/graph/context).

Seus comentários são importantes para nós. Conecte-se conosco no [Microsoft Q&A](/answers/products/m365#microsoft-graph). Marque suas perguntas com [microsoft-graph-*]
