---
title: 'Controle de versão, suporte e mudanças significativas de políticas para o Microsoft Graph '
description: Este artigo descreve o suporte e as alterações significativas de políticas do Microsoft Graph e as versões da API Microsoft Graph disponível no momento.
localization_priority: Priority
ms.openlocfilehash: 47d0ec66fc335a50826d94511c8f9e6551c927a6
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744007"
---
# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a>Controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph

Este artigo descreve o suporte e as alterações significativas de políticas do Microsoft Graph e as versões da API Microsoft Graph disponível no momento.

## <a name="support-policy-and-deprecation-information"></a>Informações de política e substituição de suporte

O Microsoft Graph segue a [Política de Ciclo de Vida da Microsoft](https://support.microsoft.com/lifecycle).

As new versions of the Microsoft Graph REST APIs and Microsoft Graph SDKs are released, earlier versions will be retired. Microsoft will declare a version as deprecated at least 24 months in advance of retiring an API or an SDK.

Quando incrementamos a versão principal da API (por exemplo, da v1.0 para a v2.0), estamos anunciando que a versão atual (neste exemplo, v1.0) está obsoleta imediatamente e não ofereceremos mais suporte 24 meses após o anúncio. Podemos fazer exceções a essa política em questões de segurança de serviço ou confiabilidade de integridade.

Quando uma API é marcada como preterida, é altamente recomendável que você migre para a versão mais recente assim que possível. Em alguns casos, anunciaremos que os novos aplicativos deverão começar a usar as novas APIs um pouco depois das APIs originais serem preteridas. Nesses casos, apenas os aplicativos ativos que usam atualmente as APIs preteridas podem continuar a usá-las.

### <a name="api-contract-and-non-backward-compatible-changes"></a>Contrato de API e alterações sem compatibilidade com versões anteriores

Microsoft Graph has a log of changes across versions. These changes are listed in the [Microsoft Graph Changelog](changelog.md). As new functionality and data is added to Microsoft Graph, we will increment the API version number for any non-backward compatible changes to the API.

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

>**Note:** Over time, we will update the list of backward compatible changes. If you generate your own client proxies (like WCF clients), our guidance is that your client applications should be prepared to receive properties and derived types not previously defined by the Microsoft Graph API service. Microsoft Graph API follows the guidance described in the [Model Versioning](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) section in the [Microsoft REST API guidelines](https://github.com/microsoft/api-guidelines/).

## <a name="versions"></a>Versões

As seguintes versões da API Microsoft Graph estão disponíveis atualmente.

### <a name="beta-version"></a>Versão beta
Exposto em `https://graph.microsoft.com/beta`, a versão beta da API Microsoft Graph contém recursos que estão atualmente _**na visualização**_. Para obter a documentação da API beta, veja [Referência de ponto de extremidade do Microsoft Graph beta](/graph/api/overview?view=graph-rest-beta). Espere alterações significativas na versão beta regularmente. Não use uma dependência de produção em APIs /beta.

We make no guarantees that a beta feature will be promoted to the current version. When the Microsoft Graph API team believes that a beta feature is ready for general availability (GA), we will add that feature to the latest current version. If the promotion of the feature would result in a breaking change to the current version, the version number will be incremented, with the new version becoming the current version.
Our developer community can post feature request on [UserVoice](https://officespdev.uservoice.com/), including requests for new features as well as requests to promote existing beta APIs to the current version.

### <a name="current-version"></a>Versão atual

The current version of Microsoft Graph is v1.0. Exposed under `https://graph.microsoft.com/v1.0`, the Microsoft Graph API /v1.0 version contains features that are generally available and ready for production use. You can browse the documentation for the v1.0 APIs in the table of contents.

### <a name="deprecated-and-unsupported-versions"></a>Versões preteridas e sem suporte

Não há atualmente nenhuma versão preterida da Microsoft Graph.

## <a name="terms-of-use"></a>Termos de uso

Ao usar as APIs do Microsoft Graph, você concorda com os [Termos de Uso das APIs da Microsoft](/legal/microsoft-apis/terms-of-use?context=/graph/context).

Your feedback is important to us. Connect with us on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your questions with [microsoft-graph].
