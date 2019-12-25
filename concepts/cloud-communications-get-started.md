---
title: Introdução às comunicações em nuvem
description: Saiba como você pode usar bots para responder às necessidades dos clientes e facilitar a colaboração.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: ae04e60079a789125dd6a818c19ec625eaac1443
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871554"
---
# <a name="get-started-with-cloud-communications"></a>Introdução às comunicações em nuvem

As APIs de comunicação em nuvem no Microsoft Graph adicionam uma nova dimensão a como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados a comunicações, como chamadas e reuniões online. Este artigo descreve como você pode usar os bots para responder às necessidades dos clientes e facilitar a colaboração.

## <a name="prerequisites"></a>Pré-requisitos

Beore você começar, será útil se familiarizar com o seguinte:

- [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) e como o serviço ajuda os funcionários a entrar e acessar recursos.
- O [serviço do Azure bot](https://docs.microsoft.com/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0) e seus recursos.

## <a name="register-a-bot"></a>Registrar um bot

Os termos "aplicativo de serviço" e "bot" podem ser usados de forma intercambiável. Você pode criar um bot através do [portal do Azure](https://azure.microsoft.com/features/azure-portal/) diretamente ou registrar um bot que não está hospedado no Azure. Para obter mais detalhes sobre o processo de registro de bot, consulte [registro de um bot de chamada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). 

Para facilitar as coisas mais tarde, é útil entender os diferentes [tipos de permissões](https://docs.microsoft.com/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) no Azure AD. Aplicativos com permissões delegadas exigem um usuário conectado. As permissões baseadas em aplicativo não precisam de um usuário conectado e geralmente podem ser executadas como um serviço em segundo plano.

Depois de registrar seu bot, se você quiser [Adicionar seu bot ao Microsoft Teams](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot), não deixe de entender como usar o [app Studio](https://docs.microsoft.com/microsoftteams/platform/get-started/get-started-app-studio) e definir os metadados necessários.

## <a name="manage-the-state-of-the-bot"></a>Gerenciar o estado do bot

Depois de registrar seu bot, decida se deseja que sua mídia baseada em áudio e vídeo seja [hospedada no aplicativo ou no serviço](cloud-communications-media.md). Em um nível alto, isso envolve decidir se você deseja ou não acessar um fluxo de mídia brutos ao vivo.

Em seguida, você pode decidir se é melhor para o bot ter estado [ou sem estado](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html).

### <a name="stateless-bots"></a>Bots sem estado

Qualquer máquina virtual pode lidar com qualquer instância de bot, o que significa que, se uma máquina for desativada, outra poderá cuidar dela. Isso torna uma solução resiliente.

Por outro lado, um cache compartilhado, como o REDIS, precisa estar acessível a todas as máquinas virtuais.

### <a name="stateful-bots"></a>Bots com estado

Uma máquina virtual pode manipular apenas uma instância de bot por vez. Como todos os Estados estão em uma máquina, não há verificações de memória extra ou verificações de cache do REDIS.

A desvantagem é que, como a instância de bot está apenas em uma máquina, ela não é tão resiliente.

>**Observação:** Os bots de mídia hospedados pelo serviço podem ter estado ou sem estado. Os bots de mídia hospedados por aplicativos devem ter estado para usar o [SDK de mídia do bot](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media).

## <a name="use-the-sdks"></a>Usar os SDKs

Os seguintes SDKs estão disponíveis em C#. Forneceremos suporte para outros idiomas no futuro.

- Se você estiver usando bots **sem estado** , instale o [SDK de núcleo de comunicações do Graph](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).
- Se você estiver usando bots com **estado** , instale o [SDK de chamada de comunicações de gráfico](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls).

## <a name="examples"></a>Exemplos

Saiba como implementar diferentes cenários usando bots stateful, como [atender a uma chamada de entrada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) com mídia hospedada por aplicativos ou por serviço.

Para obter mais exemplos, consulte o [repositório de exemplos de comunicação](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html).
