---
title: tipo de recurso convite
description: Representa um convite usado para adicionar usuários externos a uma organização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a6a009640b47ce02b1719d6e5535813d365dc9e6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450638"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="c5c6a-103">tipo de recurso convite</span><span class="sxs-lookup"><span data-stu-id="c5c6a-103">invitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5c6a-104">Representa um convite usado para adicionar usuários externos a uma organização.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-104">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="c5c6a-105">O processo de convite usa o fluxo a seguir:</span><span class="sxs-lookup"><span data-stu-id="c5c6a-105">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="c5c6a-106">Um convite é criado</span><span class="sxs-lookup"><span data-stu-id="c5c6a-106">An invitation is created</span></span>
* <span data-ttu-id="c5c6a-107">Um convite é enviado ao usuário convidado (contendo um link do convite)</span><span class="sxs-lookup"><span data-stu-id="c5c6a-107">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="c5c6a-108">O usuário convidado clica no link do convite, entra e recupera o convite, e a criação da entidade de usuário que representa o usuário convidado é concluída</span><span class="sxs-lookup"><span data-stu-id="c5c6a-108">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="c5c6a-109">O usuário é redirecionado para uma página específica após a conclusão do resgate</span><span class="sxs-lookup"><span data-stu-id="c5c6a-109">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="c5c6a-p101">A criação de um convite retornará uma URL de resgate na resposta (*inviteRedeemUrl*). A API de criação de convite pode enviar automaticamente um email que contém a URL de resgate ao usuário convidado, definindo-se *sendInvitationMessage* como true. Você também pode personalizar a mensagem será enviada ao usuário convidado. Em vez disso, se você desejar enviar a URL de resgate por outros meios, poderá definir *sendInvitationMessage* como false e usar a URL de resgate da resposta para criar sua própria comunicação. Atualmente, não há qualquer API para execução do processo de resgate. O usuário convidado tem que clicar no link *inviteRedeemUrl* enviado na comunicação na etapa anterior e passar pelo processo de resgate interativo em um navegador. Após a conclusão, o usuário convidado torna-se um usuário externo na organização.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>

>[!NOTE]
><span data-ttu-id="c5c6a-117">O status do convite é rastreado usando as propriedades **externalUserState** e **externalUserStateChangeDateTime** no recurso de [usuário](user.md) externo criado como parte da solicitação de convite.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-117">The invitation status is tracked using the **externalUserState** and the **externalUserStateChangeDateTime** properties on the external [user](user.md) resource created as part of the invitation request.</span></span>

## <a name="methods"></a><span data-ttu-id="c5c6a-118">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5c6a-118">Methods</span></span>
| <span data-ttu-id="c5c6a-119">Método</span><span class="sxs-lookup"><span data-stu-id="c5c6a-119">Method</span></span>       | <span data-ttu-id="c5c6a-120">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5c6a-120">Return Type</span></span>  |<span data-ttu-id="c5c6a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5c6a-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5c6a-122">Criar convite</span><span class="sxs-lookup"><span data-stu-id="c5c6a-122">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="c5c6a-123">invitation</span><span class="sxs-lookup"><span data-stu-id="c5c6a-123">invitation</span></span> | <span data-ttu-id="c5c6a-124">Escreva as propriedades e os relacionamentos do objeto invitation.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-124">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5c6a-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5c6a-125">Properties</span></span>
| <span data-ttu-id="c5c6a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5c6a-126">Property</span></span>     | <span data-ttu-id="c5c6a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5c6a-127">Type</span></span>   |<span data-ttu-id="c5c6a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5c6a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5c6a-129">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="c5c6a-129">invitedUserDisplayName</span></span>|<span data-ttu-id="c5c6a-130">String</span><span class="sxs-lookup"><span data-stu-id="c5c6a-130">String</span></span>|<span data-ttu-id="c5c6a-131">O nome de exibição do usuário que está sendo convidado.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-131">The display name of the user being invited.</span></span>|
|<span data-ttu-id="c5c6a-132">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c5c6a-132">invitedUserEmailAddress</span></span>|<span data-ttu-id="c5c6a-133">String</span><span class="sxs-lookup"><span data-stu-id="c5c6a-133">String</span></span>|<span data-ttu-id="c5c6a-p102">O endereço de email do usuário que está sendo convidado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="c5c6a-136">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="c5c6a-136">invitedUserMessageInfo</span></span>|[<span data-ttu-id="c5c6a-137">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="c5c6a-137">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="c5c6a-138">Configurações adicionais para a mensagem que está sendo enviada ao usuário convidado, incluindo a lista de destinatários cc, o idioma e o texto da mensagem de personalização.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-138">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="c5c6a-139">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="c5c6a-139">sendInvitationMessage</span></span>|<span data-ttu-id="c5c6a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5c6a-140">Boolean</span></span>|<span data-ttu-id="c5c6a-p103">Indica se um email deve ser enviado ao usuário que está sendo convidado ou não. O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="c5c6a-143">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="c5c6a-143">inviteRedirectUrl</span></span>|<span data-ttu-id="c5c6a-144">String</span><span class="sxs-lookup"><span data-stu-id="c5c6a-144">String</span></span>|<span data-ttu-id="c5c6a-p104">A URL para a qual o usuário deve ser redirecionado após o resgate do convite. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="c5c6a-147">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="c5c6a-147">inviteRedeemUrl</span></span>|<span data-ttu-id="c5c6a-148">String</span><span class="sxs-lookup"><span data-stu-id="c5c6a-148">String</span></span>|<span data-ttu-id="c5c6a-p105">A URL que o usuário pode usar para resgatar o convite. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c5c6a-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="c5c6a-151">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="c5c6a-151">invitedUserType</span></span>|<span data-ttu-id="c5c6a-152">String</span><span class="sxs-lookup"><span data-stu-id="c5c6a-152">String</span></span>|<span data-ttu-id="c5c6a-153">O userType do usuário que está sendo convidado.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-153">The userType of the user being invited.</span></span> <span data-ttu-id="c5c6a-154">Por padrão, é Convidado.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-154">By default, this is Guest.</span></span> <span data-ttu-id="c5c6a-155">Você pode convidar como um membro se você for administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="c5c6a-155">You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="c5c6a-156">status</span><span class="sxs-lookup"><span data-stu-id="c5c6a-156">status</span></span>|<span data-ttu-id="c5c6a-157">String</span><span class="sxs-lookup"><span data-stu-id="c5c6a-157">String</span></span>|<span data-ttu-id="c5c6a-p107">O status do convite. Valores possíveis: PendingAcceptance, Completed, InProgress, e Error</span><span class="sxs-lookup"><span data-stu-id="c5c6a-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5c6a-160">Relações</span><span class="sxs-lookup"><span data-stu-id="c5c6a-160">Relationships</span></span>
| <span data-ttu-id="c5c6a-161">Relação</span><span class="sxs-lookup"><span data-stu-id="c5c6a-161">Relationship</span></span> | <span data-ttu-id="c5c6a-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5c6a-162">Type</span></span>   |<span data-ttu-id="c5c6a-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5c6a-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5c6a-164">invitedUser</span><span class="sxs-lookup"><span data-stu-id="c5c6a-164">invitedUser</span></span>|[<span data-ttu-id="c5c6a-165">Usuário</span><span class="sxs-lookup"><span data-stu-id="c5c6a-165">user</span></span>](user.md)|<span data-ttu-id="c5c6a-p108">O usuário criado como parte da criação do convite. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c5c6a-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5c6a-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5c6a-168">JSON representation</span></span>
<span data-ttu-id="c5c6a-169">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c5c6a-169">Here is a JSON representation of the resource</span></span>

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
