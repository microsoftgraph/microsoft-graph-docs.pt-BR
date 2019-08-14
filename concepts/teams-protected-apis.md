---
title: APIs protegidas no Microsoft Teams
description: As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 124a2f96f2c59909311fad605beeb1273193d8af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364527"
---
# <a name="protected-apis-in-microsoft-teams"></a><span data-ttu-id="b7a98-103">APIs protegidas no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b7a98-103">Protected APIs in Microsoft Teams</span></span>

<span data-ttu-id="b7a98-104">As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas.</span><span class="sxs-lookup"><span data-stu-id="b7a98-104">Microsoft Teams APIs in Microsoft Graph that access sensitive data are considered protected APIs.</span></span> <span data-ttu-id="b7a98-105">Essas APIs exigem validação adicional, além de permissões e consentimento, para que você possa usá-las.</span><span class="sxs-lookup"><span data-stu-id="b7a98-105">These APIs require that you have additional validation, beyond permissions and consent, before you can use them.</span></span>

<span data-ttu-id="b7a98-106">As seguintes APIs estão protegidas no momento:</span><span class="sxs-lookup"><span data-stu-id="b7a98-106">The following APIs are currently protected:</span></span>
* <span data-ttu-id="b7a98-107">[Listar mensagens do canal](/graph/api/channel-list-messages?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="b7a98-107">[List channel messages](/graph/api/channel-list-messages?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="b7a98-108">[Receber mensagens do canal](/graph/api/channel-get-message?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="b7a98-108">[Get channel message](/graph/api/channel-get-message?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="b7a98-109">[Listar respostas a uma mensagem](/graph/api/channel-list-messagereplies?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="b7a98-109">[List replies to a message](/graph/api/channel-list-messagereplies?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="b7a98-110">[Receber resposta a uma mensagem](/graph/api/channel-get-messagereply?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="b7a98-110">[Get a reply to a message](/graph/api/channel-get-messagereply?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="b7a98-111">[Listar messagens em um chat](/graph/api/chatmessage-list?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="b7a98-111">[List messages in a chat](/graph/api/chatmessage-list?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="b7a98-112">[Receber messagens em um chat](/graph/api/chatmessage-get?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="b7a98-112">[Get message in chat](/graph/api/chatmessage-get?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>

<span data-ttu-id="b7a98-113">Para solicitar acesso a essas APIs protegidas, complete o [ formulário de solicitação](http://aka.ms/teamsgraph/requestaccess) a seguir.</span><span class="sxs-lookup"><span data-stu-id="b7a98-113">To request access to these protected APIs, complete the following [request form](http://aka.ms/teamsgraph/requestaccess).</span></span> <span data-ttu-id="b7a98-114">Analisamos as solicitações de acesso toda quarta-feira e fazemos aprovações toda sexta-feira.</span><span class="sxs-lookup"><span data-stu-id="b7a98-114">We review access requests every Wednesday and deploy approvals every Friday.</span></span>
<span data-ttu-id="b7a98-115">Caso pretenda fornecer informações além do formulário, entre em contato com o [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="b7a98-115">If you would like to provide information in addition to the form, you can contact [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span></span>
