---
title: gerenciador de convites
description: 'Use o gerenciador de convites para criar um convite para adicionar um usuário externo à organização. '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a0ee3ba23cb0c323a660b9afd26fa044a50897c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976734"
---
# <a name="invitation-manager"></a><span data-ttu-id="37a1b-103">gerenciador de convites</span><span class="sxs-lookup"><span data-stu-id="37a1b-103">invitation manager</span></span>

<span data-ttu-id="37a1b-104">Use o gerenciador de convites para criar um convite para adicionar um usuário externo à organização.</span><span class="sxs-lookup"><span data-stu-id="37a1b-104">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="37a1b-105">O processo de convite usa o fluxo a seguir:</span><span class="sxs-lookup"><span data-stu-id="37a1b-105">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="37a1b-106">Um convite é criado</span><span class="sxs-lookup"><span data-stu-id="37a1b-106">An invitation is created</span></span>
* <span data-ttu-id="37a1b-107">Um convite é enviado ao usuário convidado (contendo um link do convite)</span><span class="sxs-lookup"><span data-stu-id="37a1b-107">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="37a1b-108">O usuário convidado clica no link do convite, entra e recupera o convite, e a criação da entidade de usuário que representa o usuário convidado é concluída</span><span class="sxs-lookup"><span data-stu-id="37a1b-108">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="37a1b-109">O usuário é redirecionado para uma página específica após a conclusão do resgate</span><span class="sxs-lookup"><span data-stu-id="37a1b-109">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="37a1b-p101">A criação de um convite retornará uma URL de resgate na resposta (*inviteRedeemUrl*). A API de criação de convite pode enviar automaticamente um email que contém a URL de resgate ao usuário convidado, definindo-se *sendInvitationMessage* como true. Você também pode personalizar a mensagem será enviada ao usuário convidado. Em vez disso, se você desejar enviar a URL de resgate por outros meios, poderá definir *sendInvitationMessage* como false e usar a URL de resgate da resposta para criar sua própria comunicação. Atualmente, não há qualquer API para execução do processo de resgate. O usuário convidado tem que clicar no link *inviteRedeemUrl* enviado na comunicação na etapa anterior e passar pelo processo de resgate interativo em um navegador. Após a conclusão, o usuário convidado torna-se um usuário externo na organização.</span><span class="sxs-lookup"><span data-stu-id="37a1b-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="37a1b-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="37a1b-117">Methods</span></span>
| <span data-ttu-id="37a1b-118">Método</span><span class="sxs-lookup"><span data-stu-id="37a1b-118">Method</span></span>       | <span data-ttu-id="37a1b-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37a1b-119">Return Type</span></span>  |<span data-ttu-id="37a1b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a1b-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37a1b-121">Criar convite</span><span class="sxs-lookup"><span data-stu-id="37a1b-121">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="37a1b-122">invitation</span><span class="sxs-lookup"><span data-stu-id="37a1b-122">invitation</span></span> | <span data-ttu-id="37a1b-123">Escreva as propriedades e os relacionamentos do objeto invitation.</span><span class="sxs-lookup"><span data-stu-id="37a1b-123">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="37a1b-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37a1b-124">Properties</span></span>
| <span data-ttu-id="37a1b-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37a1b-125">Property</span></span>     | <span data-ttu-id="37a1b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="37a1b-126">Type</span></span>   |<span data-ttu-id="37a1b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a1b-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37a1b-128">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="37a1b-128">invitedUserDisplayName</span></span>|<span data-ttu-id="37a1b-129">String</span><span class="sxs-lookup"><span data-stu-id="37a1b-129">String</span></span>|<span data-ttu-id="37a1b-130">O nome de exibição do usuário que está sendo convidado.</span><span class="sxs-lookup"><span data-stu-id="37a1b-130">The display name of the user being invited.</span></span>|
|<span data-ttu-id="37a1b-131">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="37a1b-131">invitedUserEmailAddress</span></span>|<span data-ttu-id="37a1b-132">String</span><span class="sxs-lookup"><span data-stu-id="37a1b-132">String</span></span>|<span data-ttu-id="37a1b-p102">O endereço de email do usuário que está sendo convidado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a1b-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="37a1b-135">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="37a1b-135">invitedUserMessageInfo</span></span>|[<span data-ttu-id="37a1b-136">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="37a1b-136">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="37a1b-137">Configurações adicionais para a mensagem que está sendo enviada ao usuário convidado, incluindo a lista de destinatários cc, o idioma e o texto da mensagem de personalização.</span><span class="sxs-lookup"><span data-stu-id="37a1b-137">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="37a1b-138">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="37a1b-138">sendInvitationMessage</span></span>|<span data-ttu-id="37a1b-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="37a1b-139">Boolean</span></span>|<span data-ttu-id="37a1b-p103">Indica se um email deve ser enviado ao usuário que está sendo convidado ou não. O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="37a1b-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="37a1b-142">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="37a1b-142">inviteRedirectUrl</span></span>|<span data-ttu-id="37a1b-143">String</span><span class="sxs-lookup"><span data-stu-id="37a1b-143">String</span></span>|<span data-ttu-id="37a1b-p104">A URL para a qual o usuário deve ser redirecionado após o resgate do convite. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a1b-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="37a1b-146">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="37a1b-146">inviteRedeemUrl</span></span>|<span data-ttu-id="37a1b-147">String</span><span class="sxs-lookup"><span data-stu-id="37a1b-147">String</span></span>|<span data-ttu-id="37a1b-p105">A URL que o usuário pode usar para resgatar o convite. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="37a1b-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="37a1b-150">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="37a1b-150">invitedUserType</span></span>|<span data-ttu-id="37a1b-151">String</span><span class="sxs-lookup"><span data-stu-id="37a1b-151">String</span></span>|<span data-ttu-id="37a1b-152">O userType do usuário que está sendo convidado.</span><span class="sxs-lookup"><span data-stu-id="37a1b-152">The userType of the user being invited.</span></span> <span data-ttu-id="37a1b-153">Por padrão, é Convidado.</span><span class="sxs-lookup"><span data-stu-id="37a1b-153">By default, this is Guest.</span></span> <span data-ttu-id="37a1b-154">Você poderá convidar como Membro se não for administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="37a1b-154">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="37a1b-155">status</span><span class="sxs-lookup"><span data-stu-id="37a1b-155">status</span></span>|<span data-ttu-id="37a1b-156">String</span><span class="sxs-lookup"><span data-stu-id="37a1b-156">String</span></span>|<span data-ttu-id="37a1b-p107">O status do convite. Valores possíveis: PendingAcceptance, Completed, InProgress, e Error</span><span class="sxs-lookup"><span data-stu-id="37a1b-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="37a1b-159">Relações</span><span class="sxs-lookup"><span data-stu-id="37a1b-159">Relationships</span></span>
| <span data-ttu-id="37a1b-160">Relação</span><span class="sxs-lookup"><span data-stu-id="37a1b-160">Relationship</span></span> | <span data-ttu-id="37a1b-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="37a1b-161">Type</span></span>   |<span data-ttu-id="37a1b-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a1b-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37a1b-163">invitedUser</span><span class="sxs-lookup"><span data-stu-id="37a1b-163">invitedUser</span></span>|[<span data-ttu-id="37a1b-164">User</span><span class="sxs-lookup"><span data-stu-id="37a1b-164">User</span></span>](user.md)|<span data-ttu-id="37a1b-p108">O usuário criado como parte da criação do convite. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="37a1b-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37a1b-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37a1b-167">JSON representation</span></span>
<span data-ttu-id="37a1b-168">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="37a1b-168">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
