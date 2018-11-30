---
title: Usar a API do Microsoft Graph para integrar inteligência social em um aplicativo
description: O Microsoft Graph suporta gestos sociais em um contexto do usuário social e fornece acesso às pessoas útil e dados sociais.
ms.openlocfilehash: b83c5ea08c6d66dc800f736717f50324f0e2b4b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038966"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="91d70-103">Usar a API do Microsoft Graph para integrar inteligência social em um aplicativo</span><span class="sxs-lookup"><span data-stu-id="91d70-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

> <span data-ttu-id="91d70-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91d70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91d70-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91d70-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91d70-106">O Microsoft Graph suporta gestos sociais em um contexto do usuário social e fornece acesso às pessoas útil e dados sociais.</span><span class="sxs-lookup"><span data-stu-id="91d70-106">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="91d70-107">Agregadas e extrair informações específicas sobre pessoas</span><span class="sxs-lookup"><span data-stu-id="91d70-107">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="91d70-108">Use o recurso de [pessoa](../resources/person.md) e a API de pessoas para agregação de informações sobre uma pessoa em email, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="91d70-108">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="91d70-109">Os resultados são ordenados por seu relevância com base em vários relacionamentos de negócios, colaboração e comunicação.</span><span class="sxs-lookup"><span data-stu-id="91d70-109">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="91d70-110">A API permite procurar, classificar, selecione, filter ou pesquisa para as pessoas com base nos seus critérios.</span><span class="sxs-lookup"><span data-stu-id="91d70-110">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="91d70-111">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="91d70-111">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="91d70-112">Gerenciar @ menções</span><span class="sxs-lookup"><span data-stu-id="91d70-112">Manage @-Mentions</span></span>

<span data-ttu-id="91d70-113">Chamar check-out de um destinatário notificar e obter atenção do destinatário em uma mensagem é um gesto social comuns.</span><span class="sxs-lookup"><span data-stu-id="91d70-113">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="91d70-114">O recurso [mencionar](../resources/mention.md) e a API menções fornecem um mecanismo leve para destacar um destinatário em uma [mensagem](../resources/message.md), fazer todas as mensagens nas quais um usuário é notificado usando um @-mencionam ou fazer cada mencionam em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="91d70-114">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="91d70-115">Criar menções em uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="91d70-115">Create mentions in a new message</span></span>

  - [<span data-ttu-id="91d70-116">Criar e enviar menções como parte de uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="91d70-116">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="91d70-117">Criar menções como parte de um rascunho de mensagem</span><span class="sxs-lookup"><span data-stu-id="91d70-117">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="91d70-118">Obter informações sobre menções em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="91d70-118">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="91d70-119">Obtenha todas as mensagens na caixa de correio do usuário conectado que mencionam o usuário</span><span class="sxs-lookup"><span data-stu-id="91d70-119">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="91d70-120">Obter detalhes de cada menção em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="91d70-120">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="91d70-121">[Excluir um mencionam](../api/message-delete.md#request-2) em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="91d70-121">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="91d70-122">Acessar dados sociais ao redor e sobre um usuário</span><span class="sxs-lookup"><span data-stu-id="91d70-122">Access social data around and about a user</span></span>

<span data-ttu-id="91d70-123">Gráfico do Office encapsula as relações entre as entidades diferentes no Office 365.</span><span class="sxs-lookup"><span data-stu-id="91d70-123">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="91d70-124">Use o gráfico do Office para obter a ideias social para usuários individuais entre o Office 365.</span><span class="sxs-lookup"><span data-stu-id="91d70-124">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="91d70-125">Listar os itens [tendências em torno de](../api/insights-list-trending.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="91d70-125">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="91d70-126">Listar usuários que tiverem sido [Trabalhando com](../api/user-list-people.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="91d70-126">List users who have been [working with](../api/user-list-people.md) a user</span></span>
