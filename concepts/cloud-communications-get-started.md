---
title: Introdução à API de comunicações na nuvem
description: Use a API de comunicações na nuvem no Microsoft Graph para criar bots para seus clientes. Saiba como registrar seu bot e gerenciar o estado do bot.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: e2b380108d06abc987fdf92564a1ecf17289d9c5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442152"
---
# <a name="get-started-with-the-cloud-communications-api"></a>Introdução à API de comunicações na nuvem

Você pode usar a API de comunicações na nuvem no Microsoft Graph para criar bots para responder às necessidades de seus clientes e facilitar a colaboração. Este artigo descreve como registrar seu bot e gerenciar o estado do bot.

## <a name="prerequisites"></a>Pré-requisitos

Antes de começar, será útil se familiarizar com o seguinte:

- [O Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) e como o serviço ajuda os funcionários a entrar e acessar recursos.
- O [Azure Serviço de Bot](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0&preserve-view=true) e seus recursos.

## <a name="register-a-bot"></a>Registrar um bot

Os termos "aplicativo de serviço" e "bot" podem ser usados de forma intercambiável. Você pode criar um bot por meio [do portal do Azure](https://azure.microsoft.com/features/azure-portal/) diretamente ou registrar um bot que não está hospedado no Azure. Para obter mais detalhes sobre o processo de registro do bot, consulte [Registrando um bot de chamada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). 

Para facilitar as coisas mais tarde, é útil entender os diferentes tipos [de permissões](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) no Azure AD. Aplicativos com permissões delegadas exigem um usuário conectado. As permissões baseadas em aplicativo não precisam de um usuário conectado e geralmente podem ser executadas como um serviço em segundo plano.

Depois de registrar seu bot, se você quiser adicionar seu [bot ao Microsoft Teams](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot), certifique-se de entender como usar o [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) e definir os metadados necessários.

## <a name="manage-the-state-of-the-bot"></a>Gerenciar o estado do bot

Depois de registrar seu bot, decida se deseja que a mídia baseada em áudio e vídeo seja hospedada pelo aplicativo ou [pelo serviço](cloud-communications-media.md). Em um alto nível, isso envolve decidir se você deseja ou não acessar uma transmissão ao vivo de mídia bruta.

Em seguida, você pode decidir se é melhor para o bot ter estado [ou sem estado](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html).

### <a name="stateless-bots"></a>Bots sem estado

Qualquer máquina virtual pode lidar com qualquer instância de bot, o que significa que, se uma máquina falhar, outra poderá cuidar dela. Isso torna uma solução resiliente.

Por outro lado, um cache compartilhado, como REDIS, precisa estar acessível a todas as máquinas virtuais.

### <a name="stateful-bots"></a>Bots com estado

Uma máquina virtual pode manipular apenas uma instância de bot por vez. Como todos os estados estão em um computador, não há verificações de memória extras ou verificações de cache REDIS.

A desvantagem é que, como a instância do bot está apenas em um computador, ela não é tão resiliente.

> [!NOTE]
> Os bots de mídia hospedados pelo serviço podem ter estado ou sem estado. Os bots de mídia hospedados pelo aplicativo devem ter estado para usar o [SDK de Mídia do Bot](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media).

## <a name="use-the-sdks"></a>Use os SDKs

Os SDKs a seguir estão disponíveis em C#. Forneceremos suporte para outros idiomas no futuro.

- Se você estiver usando bots **sem** estado, instale o [SDK do Graph Communications Core](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).
- Se você estiver usando bots **com** estado, instale o [SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls) de Chamada de Comunicações do Graph.

## <a name="examples"></a>Exemplos

Saiba como implementar cenários diferentes usando bots com estado, como atender a [](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) uma chamada de entrada com mídia hospedada pelo aplicativo ou pelo serviço.

Para obter mais exemplos, consulte o repositório [de exemplos de Comunicações](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html).

## <a name="privacy-and-compliance"></a>Privacidade e conformidade

Nas solicitações para nossas APIs, os dados confidenciais não devem ser enviados em nenhuma ID gerada do lado do cliente (como IDs de cenário, IDs de solicitação ou outras IDs de correlação) nos cabeçalhos ou no corpo da solicitação. Essas IDs serão registradas no lado do servidor para diagnóstico.

## <a name="see-also"></a>Confira também

- [Visão geral da API de comunicações na nuvem](cloud-communications-concept-overview.md)