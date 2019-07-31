---
title: Usar a API do Microsoft Graph para integrar a inteligência social e do local de trabalho em um aplicativo
description: O Microsoft Graph dá suporte a gestos sociais em um contexto social do usuário e fornece acesso a pessoas e dados sociais úteis.
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 84e0c82173dad6f08d5911f32ef5c384f041ea19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008086"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="18716-103">Usar a API do Microsoft Graph para integrar a inteligência social e do local de trabalho em um aplicativo</span><span class="sxs-lookup"><span data-stu-id="18716-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18716-104">O Microsoft Graph dá suporte a gestos sociais em um contexto social do usuário e fornece acesso a pessoas e dados sociais úteis.</span><span class="sxs-lookup"><span data-stu-id="18716-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="18716-105">Agregar e extraia informações específicas sobre pessoas</span><span class="sxs-lookup"><span data-stu-id="18716-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="18716-106">Use o recurso [person](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="18716-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="18716-107">Os resultados são ordenados por sua relevância com base em várias relações de comunicação, colaboração e comerciais.</span><span class="sxs-lookup"><span data-stu-id="18716-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="18716-108">A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.</span><span class="sxs-lookup"><span data-stu-id="18716-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="18716-109">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="18716-109">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="18716-110">Ajudar os usuários a obter os documentos mais relevantes para seu trabalho</span><span class="sxs-lookup"><span data-stu-id="18716-110">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="18716-111">Usar a API insights para identificar os documentos mais relevantes para o usuário:</span><span class="sxs-lookup"><span data-stu-id="18716-111">Use the insights API to identify the most relevant documents for a user:</span></span> 

- <span data-ttu-id="18716-112">Listar documentos [mais populares](../api/insights-list-trending.md) de um usuário</span><span class="sxs-lookup"><span data-stu-id="18716-112">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="18716-113">Listar documentos [usados por](../api/insights-list-used.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="18716-113">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="18716-114">Listar documentos [compartilhados com ou por](../api/insights-list-shared.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="18716-114">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="18716-115">Gerenciar as @menções</span><span class="sxs-lookup"><span data-stu-id="18716-115">Manage @-Mentions</span></span>

<span data-ttu-id="18716-116">Chamar um destinatário para notificar e atrair a atenção do destinatário em uma mensagem é um gesto social comum.</span><span class="sxs-lookup"><span data-stu-id="18716-116">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="18716-117">O recurso [menção](../resources/mention.md) e a API de Menções fornecem um mecanismo simplificado para marcar um destinatário em uma [mensagem](../resources/message.md), receber todas as mensagens nas quais um usuário é notificado usando uma @menção ou receber cada menção em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="18716-117">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="18716-118">Criar menções em uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="18716-118">Create mentions in a new message</span></span>

  - [<span data-ttu-id="18716-119">Criar e enviar menções como parte de uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="18716-119">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="18716-120">Criar menções como parte de um rascunho da mensagem</span><span class="sxs-lookup"><span data-stu-id="18716-120">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="18716-121">Obter informações sobre menções em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="18716-121">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="18716-122">Obter todas as mensagens na caixa de correio do usuário conectado que mencionou o usuário</span><span class="sxs-lookup"><span data-stu-id="18716-122">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="18716-123">Obter os detalhes de cada menção em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="18716-123">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="18716-124">[Excluir uma menção](../api/message-delete.md#request-2) em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="18716-124">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

