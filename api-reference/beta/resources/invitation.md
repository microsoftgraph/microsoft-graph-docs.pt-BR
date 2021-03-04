---
title: tipo de recurso convite
description: Representa um convite usado para adicionar usuários externos a uma organização.
localization_priority: Normal
author: elisolMS
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5f132f1fb79c9f74df636b4684f6d42cdbe5bdc7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443003"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="19b10-103">tipo de recurso convite</span><span class="sxs-lookup"><span data-stu-id="19b10-103">invitation resource type</span></span>

<span data-ttu-id="19b10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19b10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19b10-105">Representa um convite usado para adicionar usuários externos a uma organização.</span><span class="sxs-lookup"><span data-stu-id="19b10-105">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="19b10-106">O processo de convite usa o fluxo a seguir:</span><span class="sxs-lookup"><span data-stu-id="19b10-106">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="19b10-107">Um convite é criado</span><span class="sxs-lookup"><span data-stu-id="19b10-107">An invitation is created</span></span>
* <span data-ttu-id="19b10-108">Um convite é enviado ao usuário convidado (contendo um link do convite)</span><span class="sxs-lookup"><span data-stu-id="19b10-108">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="19b10-109">O usuário convidado clica no link do convite, entra e recupera o convite, e a criação da entidade de usuário que representa o usuário convidado é concluída</span><span class="sxs-lookup"><span data-stu-id="19b10-109">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="19b10-110">O usuário é redirecionado para uma página específica após a conclusão do resgate</span><span class="sxs-lookup"><span data-stu-id="19b10-110">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="19b10-p101">A criação de um convite retornará uma URL de resgate na resposta (*inviteRedeemUrl*). A API de criação de convite pode enviar automaticamente um email que contém a URL de resgate ao usuário convidado, definindo-se *sendInvitationMessage* como true. Você também pode personalizar a mensagem será enviada ao usuário convidado. Em vez disso, se você desejar enviar a URL de resgate por outros meios, poderá definir *sendInvitationMessage* como false e usar a URL de resgate da resposta para criar sua própria comunicação. Atualmente, não há qualquer API para execução do processo de resgate. O usuário convidado tem que clicar no link *inviteRedeemUrl* enviado na comunicação na etapa anterior e passar pelo processo de resgate interativo em um navegador. Após a conclusão, o usuário convidado torna-se um usuário externo na organização.</span><span class="sxs-lookup"><span data-stu-id="19b10-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>

>[!NOTE]
><span data-ttu-id="19b10-118">O status do convite é rastreado usando **as propriedades externalUserState** e [](user.md) **externalUserStateChangeDateTime** no recurso de usuário externo criado como parte da solicitação de convite.</span><span class="sxs-lookup"><span data-stu-id="19b10-118">The invitation status is tracked using the **externalUserState** and the **externalUserStateChangeDateTime** properties on the external [user](user.md) resource created as part of the invitation request.</span></span>

## <a name="methods"></a><span data-ttu-id="19b10-119">Methods</span><span class="sxs-lookup"><span data-stu-id="19b10-119">Methods</span></span>
| <span data-ttu-id="19b10-120">Método</span><span class="sxs-lookup"><span data-stu-id="19b10-120">Method</span></span>       | <span data-ttu-id="19b10-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="19b10-121">Return Type</span></span>  |<span data-ttu-id="19b10-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b10-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="19b10-123">Criar convite</span><span class="sxs-lookup"><span data-stu-id="19b10-123">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="19b10-124">invitation</span><span class="sxs-lookup"><span data-stu-id="19b10-124">invitation</span></span> | <span data-ttu-id="19b10-125">Escreva as propriedades e os relacionamentos do objeto invitation.</span><span class="sxs-lookup"><span data-stu-id="19b10-125">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="19b10-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19b10-126">Properties</span></span>
| <span data-ttu-id="19b10-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19b10-127">Property</span></span>     | <span data-ttu-id="19b10-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="19b10-128">Type</span></span>   |<span data-ttu-id="19b10-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b10-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19b10-130">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="19b10-130">invitedUserDisplayName</span></span>|<span data-ttu-id="19b10-131">String</span><span class="sxs-lookup"><span data-stu-id="19b10-131">String</span></span>|<span data-ttu-id="19b10-132">O nome de exibição do usuário que está sendo convidado.</span><span class="sxs-lookup"><span data-stu-id="19b10-132">The display name of the user being invited.</span></span>|
|<span data-ttu-id="19b10-133">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="19b10-133">invitedUserEmailAddress</span></span>|<span data-ttu-id="19b10-134">String</span><span class="sxs-lookup"><span data-stu-id="19b10-134">String</span></span>|<span data-ttu-id="19b10-135">O endereço de email do usuário que está sendo convidado.</span><span class="sxs-lookup"><span data-stu-id="19b10-135">The email address of the user being invited.</span></span> <span data-ttu-id="19b10-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19b10-136">Required.</span></span> <span data-ttu-id="19b10-137">Os seguintes caracteres especiais não são permitidos no endereço de email:</span><span class="sxs-lookup"><span data-stu-id="19b10-137">The following special characters are not permitted in the email address:</span></span><br><ul><li><span data-ttu-id="19b10-138">Til (~)</span><span class="sxs-lookup"><span data-stu-id="19b10-138">Tilde (~)</span></span></li><li><span data-ttu-id="19b10-139">Ponto de exclamação (`!`)</span><span class="sxs-lookup"><span data-stu-id="19b10-139">Exclamation point (`!`)</span></span></li><li><span data-ttu-id="19b10-140">Arroba (`@`)</span><span class="sxs-lookup"><span data-stu-id="19b10-140">At sign (`@`)</span></span></li><li><span data-ttu-id="19b10-141">Hashtag (`#`)</span><span class="sxs-lookup"><span data-stu-id="19b10-141">Number sign (`#`)</span></span></li><li><span data-ttu-id="19b10-142">Cifrão (`$`)</span><span class="sxs-lookup"><span data-stu-id="19b10-142">Dollar sign (`$`)</span></span></li><li><span data-ttu-id="19b10-143">Percentagem (`%`)</span><span class="sxs-lookup"><span data-stu-id="19b10-143">Percent (`%`)</span></span></li><li><span data-ttu-id="19b10-144">Acento circunflexo (`^`)</span><span class="sxs-lookup"><span data-stu-id="19b10-144">Circumflex (`^`)</span></span></li><li><span data-ttu-id="19b10-145">E comercial (`&`)</span><span class="sxs-lookup"><span data-stu-id="19b10-145">Ampersand (`&`)</span></span></li><li><span data-ttu-id="19b10-146">Asterisco (`*`)</span><span class="sxs-lookup"><span data-stu-id="19b10-146">Asterisk (`*`)</span></span></li><li><span data-ttu-id="19b10-147">Parênteses (`( )`)</span><span class="sxs-lookup"><span data-stu-id="19b10-147">Parentheses (`( )`)</span></span></li><li><span data-ttu-id="19b10-148">Hífen (`-`)</span><span class="sxs-lookup"><span data-stu-id="19b10-148">Hyphen (`-`)</span></span></li><li><span data-ttu-id="19b10-149">Sinal de mais (`+`)</span><span class="sxs-lookup"><span data-stu-id="19b10-149">Plus sign (`+`)</span></span></li><li><span data-ttu-id="19b10-150">Sinal de igualdade (`=`)</span><span class="sxs-lookup"><span data-stu-id="19b10-150">Equal sign (`=`)</span></span></li><li><span data-ttu-id="19b10-151">Colchetes (`[ ]`)</span><span class="sxs-lookup"><span data-stu-id="19b10-151">Brackets (`[ ]`)</span></span></li><li><span data-ttu-id="19b10-152">Chaves (`{ }`)</span><span class="sxs-lookup"><span data-stu-id="19b10-152">Braces (`{ }`)</span></span></li><li><span data-ttu-id="19b10-153">Barra invertida (`\`)</span><span class="sxs-lookup"><span data-stu-id="19b10-153">Backslash (`\`)</span></span></li><li><span data-ttu-id="19b10-154">Barra (`/`)</span><span class="sxs-lookup"><span data-stu-id="19b10-154">Slash mark (`/`)</span></span></li><li><span data-ttu-id="19b10-155">Barra vertical (`|`)</span><span class="sxs-lookup"><span data-stu-id="19b10-155">Pipe (`|`)</span></span></li><li><span data-ttu-id="19b10-156">Ponto e vírgula (`;`)</span><span class="sxs-lookup"><span data-stu-id="19b10-156">Semicolon (`;`)</span></span></li><li><span data-ttu-id="19b10-157">Dois pontos (`:`)</span><span class="sxs-lookup"><span data-stu-id="19b10-157">Colon (`:`)</span></span></li><li><span data-ttu-id="19b10-158">Aspas (`"`)</span><span class="sxs-lookup"><span data-stu-id="19b10-158">Quotation marks (`"`)</span></span></li><li><span data-ttu-id="19b10-159">Sinais de maior-que e menor-que(`< >`)</span><span class="sxs-lookup"><span data-stu-id="19b10-159">Angle brackets (`< >`)</span></span></li><li><span data-ttu-id="19b10-160">Sinal de interrogação (`?`)</span><span class="sxs-lookup"><span data-stu-id="19b10-160">Question mark (`?`)</span></span></li><li><span data-ttu-id="19b10-161">Vírgula (`,`)</span><span class="sxs-lookup"><span data-stu-id="19b10-161">Comma (`,`)</span></span></li></ul><br><span data-ttu-id="19b10-162">No entanto, as seguintes exceções se aplicam:</span><span class="sxs-lookup"><span data-stu-id="19b10-162">However, the following exceptions apply:</span></span><br><ul><li><span data-ttu-id="19b10-163">Um ponto (`.`) ou um hífen (`-`) é permitido em qualquer lugar no nome de usuário, exceto no início ou no final do nome.</span><span class="sxs-lookup"><span data-stu-id="19b10-163">A period (`.`) or a hyphen (`-`) is permitted anywhere in the user name, except at the beginning or end of the name.</span></span></li><li><span data-ttu-id="19b10-164">Um underline (`_`) é permitido em qualquer lugar no nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="19b10-164">An underscore (`_`) is permitted anywhere in the user name.</span></span> <span data-ttu-id="19b10-165">Isso inclui no início ou no final do nome.</span><span class="sxs-lookup"><span data-stu-id="19b10-165">This includes at the beginning or end of the name.</span></span></li></ul>|
|<span data-ttu-id="19b10-166">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="19b10-166">invitedUserMessageInfo</span></span>|[<span data-ttu-id="19b10-167">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="19b10-167">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="19b10-168">Configurações adicionais para a mensagem que está sendo enviada ao usuário convidado, incluindo a lista de destinatários cc, o idioma e o texto da mensagem de personalização.</span><span class="sxs-lookup"><span data-stu-id="19b10-168">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="19b10-169">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="19b10-169">sendInvitationMessage</span></span>|<span data-ttu-id="19b10-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="19b10-170">Boolean</span></span>|<span data-ttu-id="19b10-p104">Indica se um email deve ser enviado ao usuário que está sendo convidado ou não. O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="19b10-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="19b10-173">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="19b10-173">inviteRedirectUrl</span></span>|<span data-ttu-id="19b10-174">String</span><span class="sxs-lookup"><span data-stu-id="19b10-174">String</span></span>|<span data-ttu-id="19b10-p105">A URL para a qual o usuário deve ser redirecionado após o resgate do convite. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19b10-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="19b10-177">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="19b10-177">inviteRedeemUrl</span></span>|<span data-ttu-id="19b10-178">String</span><span class="sxs-lookup"><span data-stu-id="19b10-178">String</span></span>|<span data-ttu-id="19b10-179">A URL que o usuário pode usar para resgatar seu convite.</span><span class="sxs-lookup"><span data-stu-id="19b10-179">The URL the user can use to redeem their invitation.</span></span> <span data-ttu-id="19b10-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="19b10-180">Read-only.</span></span>|
|<span data-ttu-id="19b10-181">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="19b10-181">invitedUserType</span></span>|<span data-ttu-id="19b10-182">String</span><span class="sxs-lookup"><span data-stu-id="19b10-182">String</span></span>|<span data-ttu-id="19b10-183">O userType do usuário que está sendo convidado.</span><span class="sxs-lookup"><span data-stu-id="19b10-183">The userType of the user being invited.</span></span> <span data-ttu-id="19b10-184">Por padrão, é Convidado.</span><span class="sxs-lookup"><span data-stu-id="19b10-184">By default, this is Guest.</span></span> <span data-ttu-id="19b10-185">Você pode convidar como Membro se for administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="19b10-185">You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="19b10-186">status</span><span class="sxs-lookup"><span data-stu-id="19b10-186">status</span></span>|<span data-ttu-id="19b10-187">String</span><span class="sxs-lookup"><span data-stu-id="19b10-187">String</span></span>|<span data-ttu-id="19b10-p108">O status do convite. Valores possíveis: PendingAcceptance, Completed, InProgress, e Error</span><span class="sxs-lookup"><span data-stu-id="19b10-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="19b10-190">Relações</span><span class="sxs-lookup"><span data-stu-id="19b10-190">Relationships</span></span>
| <span data-ttu-id="19b10-191">Relação</span><span class="sxs-lookup"><span data-stu-id="19b10-191">Relationship</span></span> | <span data-ttu-id="19b10-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="19b10-192">Type</span></span>   |<span data-ttu-id="19b10-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b10-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19b10-194">invitedUser</span><span class="sxs-lookup"><span data-stu-id="19b10-194">invitedUser</span></span>|[<span data-ttu-id="19b10-195">user</span><span class="sxs-lookup"><span data-stu-id="19b10-195">user</span></span>](user.md)|<span data-ttu-id="19b10-p109">O usuário criado como parte da criação do convite. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="19b10-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19b10-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19b10-198">JSON representation</span></span>
<span data-ttu-id="19b10-199">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="19b10-199">Here is a JSON representation of the resource</span></span>

<!-- 
{ 
    "blockType": "resource",
    "keyProperty":"id",
    "@odata.type": "microsoft.graph.invitation", 
    "optionalProperties": [
        "invitedUser"
     ],
    "baseType": "microsoft.graph.entity"
} 
-->
```json
{
  "id": "string",
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
<!--
{
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


