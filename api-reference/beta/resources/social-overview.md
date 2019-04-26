---
title: Usar a API do Microsoft Graph para integrar a inteligência social em um aplicativo
description: O Microsoft Graph dá suporte a gestos sociais em um contexto social do usuário e fornece acesso a pessoas e dados sociais úteis.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 45482d2e47c97b6c09302ab60ff9c031cef1e92a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345676"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="8dfb6-103">Usar a API do Microsoft Graph para integrar a inteligência social em um aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dfb6-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dfb6-104">O Microsoft Graph dá suporte a gestos sociais em um contexto social do usuário e fornece acesso a pessoas e dados sociais úteis.</span><span class="sxs-lookup"><span data-stu-id="8dfb6-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="8dfb6-105">Agregar e extraia informações específicas sobre pessoas</span><span class="sxs-lookup"><span data-stu-id="8dfb6-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="8dfb6-106">Use o recurso [person](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="8dfb6-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="8dfb6-107">Os resultados são ordenados por sua relevância com base em várias relações de comunicação, colaboração e comerciais.</span><span class="sxs-lookup"><span data-stu-id="8dfb6-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="8dfb6-108">A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.</span><span class="sxs-lookup"><span data-stu-id="8dfb6-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="8dfb6-109">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="8dfb6-109">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="8dfb6-110">Gerenciar as @menções</span><span class="sxs-lookup"><span data-stu-id="8dfb6-110">Manage @-Mentions</span></span>

<span data-ttu-id="8dfb6-111">Chamar um destinatário para notificar e atrair a atenção do destinatário em uma mensagem é um gesto social comum.</span><span class="sxs-lookup"><span data-stu-id="8dfb6-111">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="8dfb6-112">O recurso [menção](../resources/mention.md) e a API de Menções fornecem um mecanismo simplificado para marcar um destinatário em uma [mensagem](../resources/message.md), receber todas as mensagens nas quais um usuário é notificado usando uma @menção ou receber cada menção em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="8dfb6-112">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="8dfb6-113">Criar menções em uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="8dfb6-113">Create mentions in a new message</span></span>

  - [<span data-ttu-id="8dfb6-114">Criar e enviar menções como parte de uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="8dfb6-114">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="8dfb6-115">Criar menções como parte de um rascunho da mensagem</span><span class="sxs-lookup"><span data-stu-id="8dfb6-115">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="8dfb6-116">Obter informações sobre menções em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="8dfb6-116">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="8dfb6-117">Obter todas as mensagens na caixa de correio do usuário conectado que mencionou o usuário</span><span class="sxs-lookup"><span data-stu-id="8dfb6-117">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="8dfb6-118">Obter os detalhes de cada menção em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="8dfb6-118">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="8dfb6-119">[Excluir uma menção](../api/message-delete.md#request-2) em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="8dfb6-119">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="8dfb6-120">Acessar dados sociais em torno e sobre um usuário</span><span class="sxs-lookup"><span data-stu-id="8dfb6-120">Access social data around and about a user</span></span>

<span data-ttu-id="8dfb6-121">O Office Graph encapsula as relações entre diferentes entidades no Office 365.</span><span class="sxs-lookup"><span data-stu-id="8dfb6-121">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="8dfb6-122">Use o Office Graph para obter informações sociais sobre usuários individuais no Office 365.</span><span class="sxs-lookup"><span data-stu-id="8dfb6-122">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="8dfb6-123">Listar os itens de [tendência em torno](../api/insights-list-trending.md) de um usuário</span><span class="sxs-lookup"><span data-stu-id="8dfb6-123">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="8dfb6-124">Listar usuários que têm [trabalhado com](../api/user-list-people.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="8dfb6-124">List users who have been [working with](../api/user-list-people.md) a user</span></span>
