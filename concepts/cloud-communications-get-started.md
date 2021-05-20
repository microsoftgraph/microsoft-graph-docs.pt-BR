---
title: Comece com comunicações em nuvem
description: Saiba como usar bots para responder às necessidades de seus clientes e facilitar a colaboração.
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
# <a name="get-started-with-cloud-communications"></a>Comece com comunicações em nuvem

As APIs de comunicação em nuvem na Microsoft Graph adicionam uma nova dimensão à forma como seus aplicativos e serviços interagem com os usuários através de vários recursos relacionados a comunicações, como chamadas e reuniões online. Este artigo descreve como você pode usar bots para responder às necessidades de seus clientes e facilitar a colaboração.

## <a name="prerequisites"></a>Pré-requisitos

Antes de começar, será útil se familiarizar com o seguinte:

- [Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) e como o serviço ajuda os funcionários a entrar e acessar recursos.
- O [Serviço Azure Bot](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0) e suas capacidades.

## <a name="register-a-bot"></a>Registre um bot

Os termos "aplicativo de serviço" e "bot" podem ser usados de forma intercambiável. Você pode criar um bot através do [portal Azure](https://azure.microsoft.com/features/azure-portal/) diretamente ou registrar um bot que não está hospedado no Azure. Para obter mais detalhes sobre o processo de registro de bots, consulte [Registrando um bot de chamada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). 

Para tornar as coisas mais fáceis mais tarde, é útil entender os [diferentes tipos de permissões](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) dentro do Azure AD. Aplicativos com permissões delegadas exigem um usuário de assinatura. As permissões baseadas em aplicativos não precisam de um usuário de assinatura e muitas vezes podem ser executadas como um serviço de antecedentes.

Depois de registrar seu bot, se quiser [adicionar seu bot a Microsoft Teams,](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)certifique-se de entender como usar o estúdio do [aplicativo](/microsoftteams/platform/get-started/get-started-app-studio) e defina os metadados necessários.

## <a name="manage-the-state-of-the-bot"></a>Gerencie o estado do bot

Depois de registrar seu bot, decida se deseja que sua mídia baseada em áudio e vídeo seja [hospedada por aplicativos ou hospedada em serviço](cloud-communications-media.md). Em alto nível, isso envolve decidir se você quer ou não acessar uma transmissão ao vivo de mídia crua.

Em seguida, você pode decidir se é melhor para o seu bot ser [apátrida ou apátrida](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html).

### <a name="stateless-bots"></a>Bots apátridas

Qualquer máquina virtual pode lidar com qualquer instância de bot, o que significa que se uma máquina cair, outra pode cuidar dela. Isso torna uma solução resiliente.

Por outro lado, um cache compartilhado, como o REDIS, precisa ser acessível a todas as máquinas virtuais.

### <a name="stateful-bots"></a>Bots imponentes

Uma máquina virtual pode lidar com apenas uma instância de bot por vez. Como todos os estados estão em uma máquina, não há verificações extras de memória ou verificações de cache REDIS.

A desvantagem é que, como a instância do bot está apenas em uma máquina, não é tão resistente.

>**Nota:** Os bots de mídia hospedados no serviço podem ser imponentes ou apátridas. Os bots de mídia hospedados por aplicativos devem ser imponentes para usar o [Bot Media SDK](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media).

## <a name="use-the-sdks"></a>Use os SDKs

Os seguintes SDKs estão disponíveis em C#. Forneceremos suporte para outras línguas no futuro.

- Se estiver usando bots **apátridas,** instale o [Graph Communications Core SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).
- Se você estiver usando bots **stateful,** instale o [Graph Communications Calling SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls).

## <a name="examples"></a>Exemplos

Aprenda a implementar diferentes cenários usando bots estatais, como [responder a uma chamada recebida](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) com mídia hospedada por aplicativos ou hospedada por serviços.

Para obter mais exemplos, consulte o [repositório de amostras de Comunicações](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html).

## <a name="privacy-and-compliance"></a>Privacidade e conformidade

Nas solicitações às nossas APIs, dados confidenciais não devem ser enviados em quaisquer IDs gerados pelo lado do cliente (como IDs de cenário, IDs de solicitação ou outras IDs de correlação) em cabeçalhos ou no órgão de solicitação. Esses IDs serão registrados no lado do servidor para diagnósticos.
