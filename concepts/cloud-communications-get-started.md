---
title: Começar a trabalhar com comunicações na nuvem
description: Saiba como você pode usar bots para responder às necessidades de seus clientes e facilitar a colaboração.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: a1c2ff420df58be8345924c2c6622f7cc6647551
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579680"
---
# <a name="get-started-with-cloud-communications"></a>Começar a trabalhar com comunicações na nuvem

As APIs de comunicações na nuvem na Microsoft Graph adicionar uma nova dimensão à forma como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados a comunicações, como chamada e reuniões online. Este artigo descreve como você pode usar bots para responder às necessidades de seus clientes e facilitar a colaboração.

## <a name="prerequisites"></a>Pré-requisitos

Antes de começar, será útil familiarizar-se com o seguinte:

- [Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) e como o serviço ajuda os funcionários a entrar e acessar recursos.
- O [Serviço bot do Azure](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0) e seus recursos.

## <a name="register-a-bot"></a>Registrar um bot

Os termos "aplicativo de serviço" e "bot" podem ser usados de forma intercambiável. Você pode criar um bot por meio do [portal do Azure](https://azure.microsoft.com/features/azure-portal/) diretamente ou registrar um bot que não está hospedado no Azure. Para obter mais detalhes sobre o processo de registro do bot, consulte [Registrando um bot de chamada.](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html) 

Para facilitar as coisas mais tarde, é útil entender os diferentes tipos de [permissões](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) no Azure AD. Os aplicativos com permissões delegadas exigem um usuário in-locar. As permissões baseadas em aplicativos não precisam de um usuário in-locado e geralmente podem ser executados como um serviço em segundo plano.

Depois de registrar seu bot, se quiser adicionar seu [bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)ao Microsoft Teams , entenda como usar o app [studio](/microsoftteams/platform/get-started/get-started-app-studio) e defina os metadados necessários.

## <a name="manage-the-state-of-the-bot"></a>Gerenciar o estado do bot

Depois de registrar seu bot, decida se deseja que sua mídia baseada em áudio e vídeo seja hospedada pelo aplicativo ou [pelo serviço.](cloud-communications-media.md) Em um nível alto, isso envolve decidir se você deseja ou não acessar um fluxo ao vivo de mídia bruta.

Em seguida, você pode decidir se é melhor para o bot ser [stateful ou stateless](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html).

### <a name="stateless-bots"></a>Bots sem estado

Qualquer máquina virtual pode manipular qualquer instância de bot, o que significa que, se uma máquina cair, outra poderá cuidar dela. Isso torna uma solução resiliente.

Por outro lado, um cache compartilhado, como REDIS, precisa estar acessível a todas as máquinas virtuais.

### <a name="stateful-bots"></a>Bots stateful

Uma máquina virtual pode manipular apenas uma instância de bot por vez. Como todos os estados estão em um computador, não há nenhuma verificação de memória extra ou verificações de cache REDIS.

A desvantagem é que, como a instância do bot está apenas em um computador, ela não é tão resiliente.

>**Observação:** Os bots de mídia hospedados pelo serviço podem ser stateful ou stateless. Os bots de mídia hospedados pelo aplicativo devem ter estado para usar o [SDK](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media)de Mídia bot .

## <a name="use-the-sdks"></a>Use os SDKs

Os SDKs a seguir estão disponíveis no C#. Forneceremos suporte para outros idiomas no futuro.

- Se você estiver usando bots **sem** estado, instale o [Graph SDK do Communications Core](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).
- Se você estiver usando bots **de** estado, instale o SDK de chamada Graph [Comunicações.](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)

## <a name="examples"></a>Exemplos

Saiba como implementar diferentes cenários usando bots de estado, como atender [uma](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) chamada de entrada com mídia hospedada por aplicativo ou hospedada pelo serviço.

Para obter mais exemplos, consulte o repositório [de exemplos de comunicações](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html).

## <a name="privacy-and-compliance"></a>Privacidade e conformidade

Nas solicitações para nossas APIs, os dados confidenciais não devem ser enviados em IDs geradas no lado do cliente (como IDs de cenário, IDs de solicitação ou outras IDs de correlação) nos headers ou no corpo da solicitação. Essas IDs serão registradas no lado do servidor para diagnóstico.
