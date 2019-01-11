---
title: gerenciador de convites
description: 'Use o gerenciador de convites para criar um convite para adicionar um usuário externo à organização. '
localization_priority: Normal
ms.openlocfilehash: ffe09e5043b60b01728d497b88034b289bdc5131
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811239"
---
# <a name="invitation-manager"></a><span data-ttu-id="0e8ca-103">gerenciador de convites</span><span class="sxs-lookup"><span data-stu-id="0e8ca-103">invitation manager</span></span>

> <span data-ttu-id="0e8ca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e8ca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e8ca-106">Use o gerenciador de convites para criar um convite para adicionar um usuário externo à organização.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-106">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="0e8ca-107">O processo de convite usa o fluxo a seguir:</span><span class="sxs-lookup"><span data-stu-id="0e8ca-107">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="0e8ca-108">Um convite é criado</span><span class="sxs-lookup"><span data-stu-id="0e8ca-108">An invitation is created</span></span>
* <span data-ttu-id="0e8ca-109">Um convite é enviado ao usuário convidado (contendo um link do convite)</span><span class="sxs-lookup"><span data-stu-id="0e8ca-109">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="0e8ca-110">O usuário convidado clica no link do convite, entra e recupera o convite, e a criação da entidade de usuário que representa o usuário convidado é concluída</span><span class="sxs-lookup"><span data-stu-id="0e8ca-110">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="0e8ca-111">O usuário é redirecionado para uma página específica após a conclusão do resgate</span><span class="sxs-lookup"><span data-stu-id="0e8ca-111">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="0e8ca-p102">A criação de um convite retornará uma URL de resgate na resposta (*inviteRedeemUrl*). A API de criação de convite pode enviar automaticamente um email que contém a URL de resgate ao usuário convidado, definindo-se *sendInvitationMessage* como true. Você também pode personalizar a mensagem será enviada ao usuário convidado. Em vez disso, se você desejar enviar a URL de resgate por outros meios, poderá definir *sendInvitationMessage* como false e usar a URL de resgate da resposta para criar sua própria comunicação. Atualmente, não há qualquer API para execução do processo de resgate. O usuário convidado tem que clicar no link *inviteRedeemUrl* enviado na comunicação na etapa anterior e passar pelo processo de resgate interativo em um navegador. Após a conclusão, o usuário convidado torna-se um usuário externo na organização.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-p102">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="0e8ca-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="0e8ca-119">Methods</span></span>
| <span data-ttu-id="0e8ca-120">Método</span><span class="sxs-lookup"><span data-stu-id="0e8ca-120">Method</span></span>       | <span data-ttu-id="0e8ca-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e8ca-121">Return Type</span></span>  |<span data-ttu-id="0e8ca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e8ca-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e8ca-123">Criar convite</span><span class="sxs-lookup"><span data-stu-id="0e8ca-123">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="0e8ca-124">invitation</span><span class="sxs-lookup"><span data-stu-id="0e8ca-124">invitation</span></span> | <span data-ttu-id="0e8ca-125">Escreva as propriedades e os relacionamentos do objeto invitation.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-125">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e8ca-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e8ca-126">Properties</span></span>
| <span data-ttu-id="0e8ca-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e8ca-127">Property</span></span>     | <span data-ttu-id="0e8ca-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e8ca-128">Type</span></span>   |<span data-ttu-id="0e8ca-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e8ca-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e8ca-130">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="0e8ca-130">invitedUserDisplayName</span></span>|<span data-ttu-id="0e8ca-131">String</span><span class="sxs-lookup"><span data-stu-id="0e8ca-131">String</span></span>|<span data-ttu-id="0e8ca-132">O nome de exibição do usuário que está sendo convidado.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-132">The display name of the user being invited.</span></span>|
|<span data-ttu-id="0e8ca-133">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0e8ca-133">invitedUserEmailAddress</span></span>|<span data-ttu-id="0e8ca-134">String</span><span class="sxs-lookup"><span data-stu-id="0e8ca-134">String</span></span>|<span data-ttu-id="0e8ca-p103">O endereço de email do usuário que está sendo convidado. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-p103">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="0e8ca-137">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="0e8ca-137">invitedUserMessageInfo</span></span>|[<span data-ttu-id="0e8ca-138">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="0e8ca-138">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="0e8ca-139">Configurações adicionais para a mensagem que está sendo enviada ao usuário convidado, incluindo a lista de destinatários cc, o idioma e o texto da mensagem de personalização.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-139">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="0e8ca-140">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="0e8ca-140">sendInvitationMessage</span></span>|<span data-ttu-id="0e8ca-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="0e8ca-141">Boolean</span></span>|<span data-ttu-id="0e8ca-p104">Indica se um email deve ser enviado ao usuário que está sendo convidado ou não. O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="0e8ca-144">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="0e8ca-144">inviteRedirectUrl</span></span>|<span data-ttu-id="0e8ca-145">String</span><span class="sxs-lookup"><span data-stu-id="0e8ca-145">String</span></span>|<span data-ttu-id="0e8ca-p105">A URL para a qual o usuário deve ser redirecionado após o resgate do convite. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="0e8ca-148">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="0e8ca-148">inviteRedeemUrl</span></span>|<span data-ttu-id="0e8ca-149">String</span><span class="sxs-lookup"><span data-stu-id="0e8ca-149">String</span></span>|<span data-ttu-id="0e8ca-p106">A URL que o usuário pode usar para resgatar o convite. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="0e8ca-p106">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="0e8ca-152">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="0e8ca-152">invitedUserType</span></span>|<span data-ttu-id="0e8ca-153">String</span><span class="sxs-lookup"><span data-stu-id="0e8ca-153">String</span></span>|<span data-ttu-id="0e8ca-p107">O userType do usuário que está sendo convidado. Por padrão, é Convidado. Você pode convidar como Membro se não for administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="0e8ca-p107">The userType of the user being invited. By default, this is Guest. You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="0e8ca-157">status</span><span class="sxs-lookup"><span data-stu-id="0e8ca-157">status</span></span>|<span data-ttu-id="0e8ca-158">String</span><span class="sxs-lookup"><span data-stu-id="0e8ca-158">String</span></span>|<span data-ttu-id="0e8ca-p108">O status do convite. Valores possíveis: PendingAcceptance, Completed, InProgress, e Error</span><span class="sxs-lookup"><span data-stu-id="0e8ca-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e8ca-161">Relações</span><span class="sxs-lookup"><span data-stu-id="0e8ca-161">Relationships</span></span>
| <span data-ttu-id="0e8ca-162">Relação</span><span class="sxs-lookup"><span data-stu-id="0e8ca-162">Relationship</span></span> | <span data-ttu-id="0e8ca-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e8ca-163">Type</span></span>   |<span data-ttu-id="0e8ca-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e8ca-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e8ca-165">invitedUser</span><span class="sxs-lookup"><span data-stu-id="0e8ca-165">invitedUser</span></span>|[<span data-ttu-id="0e8ca-166">User</span><span class="sxs-lookup"><span data-stu-id="0e8ca-166">User</span></span>](user.md)|<span data-ttu-id="0e8ca-p109">O usuário criado como parte da criação do convite. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="0e8ca-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e8ca-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e8ca-169">JSON representation</span></span>
<span data-ttu-id="0e8ca-170">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0e8ca-170">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
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
