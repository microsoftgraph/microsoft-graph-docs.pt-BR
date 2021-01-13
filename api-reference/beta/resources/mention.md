---
title: mencionar tipo de recurso
description: Representa uma notificação para uma pessoa com base no endereço de email da pessoa.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 23d4ac1d98a65e206a476768569cca89fb295a61
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844855"
---
# <a name="mention-resource-type"></a><span data-ttu-id="b2000-103">mencionar tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="b2000-103">mention resource type</span></span>

<span data-ttu-id="b2000-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2000-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2000-105">Representa uma notificação para uma pessoa com base no endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="b2000-105">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="b2000-106">Esse tipo de notificação também é conhecido como @menções.</span><span class="sxs-lookup"><span data-stu-id="b2000-106">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="b2000-107">O [recurso de](../resources/message.md) mensagem é compatível com **menção.**</span><span class="sxs-lookup"><span data-stu-id="b2000-107">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="b2000-108">Ele inclui uma **propriedade mentionsPreview** que indica se o usuário assinado é mencionado nessa instância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b2000-108">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="b2000-109">Ele também inclui a propriedade **de navegação de** menções, que oferece suporte para obter detalhes de uma menção ou excluir uma menção nessa instância.</span><span class="sxs-lookup"><span data-stu-id="b2000-109">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="b2000-110">Ao criar uma mensagem, um aplicativo pode criar uma menção na mesma solicitação incluindo a `POST` menção na propriedade **menções.**</span><span class="sxs-lookup"><span data-stu-id="b2000-110">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="b2000-111">Usando uma solicitação com o parâmetro de consulta, um aplicativo pode retornar todas as mensagens na caixa de correio do usuário que menciona `GET` `$filter` o usuário.</span><span class="sxs-lookup"><span data-stu-id="b2000-111">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="b2000-112">Uma `GET` solicitação com `$expand` o parâmetro de consulta permite que o aplicativo expanda todas as menções em uma mensagem específica.</span><span class="sxs-lookup"><span data-stu-id="b2000-112">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="b2000-113">Esse mecanismo de permitir que um aplicativo seja definido e receba menções em mensagens permite notificações leves, em que o usuário que faz a menção pode permanecer no contexto existente (como compor um corpo de mensagem) enquanto o aplicativo define a propriedade de menções **subjacentes.**</span><span class="sxs-lookup"><span data-stu-id="b2000-113">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="b2000-114">As pessoas mencionadas podem facilmente descobrir se e onde são mencionadas por meio de `GET` solicitações com `$filter` o parâmetro `$expand` ou consulta.</span><span class="sxs-lookup"><span data-stu-id="b2000-114">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="b2000-115">Por exemplo, no cliente de email do Outlook, quando um usuário digita enquanto escreve uma mensagem, o Outlook permite que o usuário selecione ou insira um nome para concluir `@` a @menção.</span><span class="sxs-lookup"><span data-stu-id="b2000-115">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="b2000-116">O Outlook define **a propriedade de menções** antes de criar e enviar a mensagem ou o evento.</span><span class="sxs-lookup"><span data-stu-id="b2000-116">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="b2000-117">Outlook also uses `GET` operations with and to let the `$filter` `$expand` signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span><span class="sxs-lookup"><span data-stu-id="b2000-117">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b2000-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2000-118">JSON representation</span></span>

<span data-ttu-id="b2000-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2000-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a><span data-ttu-id="b2000-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2000-120">Properties</span></span>
| <span data-ttu-id="b2000-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2000-121">Property</span></span>     | <span data-ttu-id="b2000-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2000-122">Type</span></span>   |<span data-ttu-id="b2000-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2000-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2000-124">application</span><span class="sxs-lookup"><span data-stu-id="b2000-124">application</span></span> | <span data-ttu-id="b2000-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2000-125">String</span></span> | <span data-ttu-id="b2000-126">O nome do aplicativo onde a menção foi criada.</span><span class="sxs-lookup"><span data-stu-id="b2000-126">The name of the application where the mention is created.</span></span> <span data-ttu-id="b2000-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b2000-127">Optional.</span></span> <span data-ttu-id="b2000-128">Não usado e padrão como nulo para **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="b2000-128">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="b2000-129">clientReference</span><span class="sxs-lookup"><span data-stu-id="b2000-129">clientReference</span></span> | <span data-ttu-id="b2000-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2000-130">String</span></span> | <span data-ttu-id="b2000-131">Um identificador exclusivo que representa um pai da instância do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2000-131">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="b2000-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b2000-132">Optional.</span></span> <span data-ttu-id="b2000-133">Não usado e padrão como nulo para **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="b2000-133">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="b2000-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="b2000-134">createdBy</span></span>  | [<span data-ttu-id="b2000-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b2000-135">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="b2000-136">As informações de email do usuário que fez a menção.</span><span class="sxs-lookup"><span data-stu-id="b2000-136">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="b2000-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2000-137">createdDateTime</span></span>  |<span data-ttu-id="b2000-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2000-138">DateTimeOffset</span></span> |<span data-ttu-id="b2000-139">A data e a hora em que a menção é criada no cliente.</span><span class="sxs-lookup"><span data-stu-id="b2000-139">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="b2000-140">deepLink</span><span class="sxs-lookup"><span data-stu-id="b2000-140">deepLink</span></span> | <span data-ttu-id="b2000-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2000-141">String</span></span> | <span data-ttu-id="b2000-142">Um link da Web profundo para o contexto da menção na instância do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2000-142">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="b2000-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b2000-143">Optional.</span></span> <span data-ttu-id="b2000-144">Não usado e padrão como nulo para **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="b2000-144">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="b2000-145">id</span><span class="sxs-lookup"><span data-stu-id="b2000-145">id</span></span> | <span data-ttu-id="b2000-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2000-146">String</span></span>| <span data-ttu-id="b2000-147">O identificador exclusivo de uma menção em uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="b2000-147">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="b2000-148">mencionado</span><span class="sxs-lookup"><span data-stu-id="b2000-148">mentioned</span></span> | [<span data-ttu-id="b2000-149">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b2000-149">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="b2000-150">As informações de email da pessoa mencionada.</span><span class="sxs-lookup"><span data-stu-id="b2000-150">The email information of the mentioned person.</span></span> <span data-ttu-id="b2000-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2000-151">Required.</span></span> |
|<span data-ttu-id="b2000-152">mentionText</span><span class="sxs-lookup"><span data-stu-id="b2000-152">mentionText</span></span> | <span data-ttu-id="b2000-153">String</span><span class="sxs-lookup"><span data-stu-id="b2000-153">String</span></span> | <span data-ttu-id="b2000-154">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b2000-154">Optional.</span></span> <span data-ttu-id="b2000-155">Não usado e padrão como nulo para **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="b2000-155">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="b2000-156">Para obter as menções em uma mensagem, consulte a **propriedade bodyPreview** da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b2000-156">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="b2000-157">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2000-157">serverCreatedDateTime</span></span> | <span data-ttu-id="b2000-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2000-158">DateTimeOffset</span></span> | <span data-ttu-id="b2000-159">A data e a hora em que a menção é criada no servidor.</span><span class="sxs-lookup"><span data-stu-id="b2000-159">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="b2000-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b2000-160">Optional.</span></span> <span data-ttu-id="b2000-161">Não usado e padrão como nulo para **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="b2000-161">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b2000-162">Relações</span><span class="sxs-lookup"><span data-stu-id="b2000-162">Relationships</span></span>
<span data-ttu-id="b2000-163">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b2000-163">None</span></span>


## <a name="methods"></a><span data-ttu-id="b2000-164">Métodos</span><span class="sxs-lookup"><span data-stu-id="b2000-164">Methods</span></span>

| <span data-ttu-id="b2000-165">Método</span><span class="sxs-lookup"><span data-stu-id="b2000-165">Method</span></span>           | <span data-ttu-id="b2000-166">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b2000-166">Return Type</span></span>    |<span data-ttu-id="b2000-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2000-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2000-168">[Postar](../api/user-sendmail.md#request-2) e enviar</span><span class="sxs-lookup"><span data-stu-id="b2000-168">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="b2000-169">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2000-169">None</span></span> | <span data-ttu-id="b2000-170">Criar e enviar menções como parte de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="b2000-170">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="b2000-171">[Postar](../api/user-post-messages.md#request-2) em um novo rascunho</span><span class="sxs-lookup"><span data-stu-id="b2000-171">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="b2000-172">[que](../resources/message.md) contém um ou mais objetos **de menção.**</span><span class="sxs-lookup"><span data-stu-id="b2000-172">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="b2000-173">Crie um rascunho de uma nova mensagem e inclua um ou mais objetos **de menção.**</span><span class="sxs-lookup"><span data-stu-id="b2000-173">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="b2000-174">[Obter](../api/user-list-messages.md#request-2) mensagens mencionando-me</span><span class="sxs-lookup"><span data-stu-id="b2000-174">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="b2000-175">Coleção [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="b2000-175">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="b2000-176">Obter todas as mensagens na caixa de correio do usuário que contêm **uma** menção a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="b2000-176">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="b2000-177">[Obter](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message) uma mensagem e suas menções</span><span class="sxs-lookup"><span data-stu-id="b2000-177">[Get](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message) a message and its mentions</span></span> | <span data-ttu-id="b2000-178">Coleção [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="b2000-178">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="b2000-179">Obter uma mensagem e expandir os detalhes de **cada menção** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="b2000-179">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="b2000-180">[Excluir](../api/message-delete.md#request-2) uma menção</span><span class="sxs-lookup"><span data-stu-id="b2000-180">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="b2000-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2000-181">None</span></span> |<span data-ttu-id="b2000-182">Exclui a menção especificada na mensagem especificada na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b2000-182">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


