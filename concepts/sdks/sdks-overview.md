---
title: Visão geral dos SDKs de Microsoft Graph
description: Descreve os SDKs disponíveis, os idiomas aos quais eles dão suporte e o valor que eles fornecem aos desenvolvedores.
ms.localizationpriority: medium
author: MichaelMainer
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9fdd4d5cc858413b08ff4f86c2b564611617c315
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060539"
---
# <a name="microsoft-graph-sdks-overview"></a>Visão geral dos SDKs de Microsoft Graph

Os SDKs do Microsoft Graph foram projetados para simplificar a criação de aplicativos de alta qualidade, eficientes e resilientes que acessam o Microsoft Graph. Os SDKs incluem dois componentes: uma biblioteca de serviços e uma biblioteca principal.

A  biblioteca de serviços contém modelos e construtores de solicitação gerados a partir dos metadados do Microsoft Graph para fornecer uma experiência avançada, fortemente tipada e detectável ao trabalhar com os muitos conjuntos de dados disponíveis no Microsoft Graph.

A *biblioteca principal* fornece um conjunto de recursos que aprimoram o trabalho com todos os serviços de Graph Microsoft. O suporte inserido para tratamento de repetição, redirecionamentos seguros, autenticação transparente e compactação de conteúdo melhora a qualidade das interações do aplicativo com o Microsoft Graph, sem nenhuma complexidade adicional, deixando você completamente no controle. A biblioteca principal também dá suporte a tarefas comuns, como paginação por meio de coleções e criação de solicitações em lote.

## <a name="supported-languages"></a>Idiomas compatíveis

No momento, os SDKs estão disponíveis para os seguintes idiomas:

- [C#](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [PowerShell](https://github.com/microsoftgraph/msgraph-sdk-powershell)
- [TypeScript | Javascript](https://github.com/microsoftgraph/msgraph-sdk-javascript)
- [Java](https://github.com/microsoftgraph/msgraph-sdk-java)
- [Ir](https://github.com/microsoftgraph/msgraph-sdk-go)
- [PHP](https://github.com/microsoftgraph/msgraph-sdk-php)
- [Python (versão prévia)](https://github.com/microsoftgraph/msgraph-sdk-python-core)
- [Objective-C | Swift](https://github.com/microsoftgraph/msgraph-sdk-objc)

## <a name="microsoft-365-developer-subscription"></a>Microsoft 365 de desenvolvedor

Ao criar aplicativos usando o Microsoft Graph, recomendamos que você obtenha uma assinatura Microsoft 365 desenvolvedor gratuita ins Microsoft 365 [Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).

## <a name="see-also"></a>Confira também

* Para obter mais detalhes sobre os recursos e as funcionalidades do SDK, consulte a documentação de requisitos de [design do](https://github.com/microsoftgraph/msgraph-sdk-design) SDK.
* Solicite ou vote em recursos adicionais no fórum [Microsoft 365 ideias da Plataforma do Desenvolvedor](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph). 
* Para obter uma lista de exemplos do Microsoft Graph, consulte a [página de Graph microsoft](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples).
