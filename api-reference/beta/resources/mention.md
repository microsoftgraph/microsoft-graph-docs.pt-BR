---
title: tipo de recurso mencionam
description: Representa uma notificação para uma pessoa com base no endereço de email da pessoa.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8e04722edf878b4f3851de837908dc5c0a02de7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523194"
---
# <a name="mention-resource-type"></a><span data-ttu-id="0d757-103">tipo de recurso mencionam</span><span class="sxs-lookup"><span data-stu-id="0d757-103">mention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d757-104">Representa uma notificação para uma pessoa com base no endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="0d757-104">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="0d757-105">Esse tipo de notificação é também conhecido como @ menções.</span><span class="sxs-lookup"><span data-stu-id="0d757-105">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="0d757-106">O recurso de [mensagem](../resources/message.md) suporta **mencionar**.</span><span class="sxs-lookup"><span data-stu-id="0d757-106">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="0d757-107">Ela inclui uma propriedade **mentionsPreview** que indica se o usuário entrou no mencionada nessa instância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="0d757-107">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="0d757-108">Ele também inclui a propriedade de navegação **menções** , que oferece suporte para obter detalhes de um mencionam ou excluindo um mencionam nesse caso.</span><span class="sxs-lookup"><span data-stu-id="0d757-108">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="0d757-109">Ao criar uma mensagem, um aplicativo pode criar um mencionam na mesma `POST` solicitação, incluindo o mencionam na propriedade **menções** .</span><span class="sxs-lookup"><span data-stu-id="0d757-109">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="0d757-110">Usando um `GET` solicitar com o `$filter` parâmetro de consulta, um aplicativo pode retornar todas as mensagens na caixa de correio do usuário conectado que mencionam o usuário.</span><span class="sxs-lookup"><span data-stu-id="0d757-110">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="0d757-111">Uma `GET` solicitar com o `$expand` consulta parâmetro permite que o aplicativo expandir todas as menções em uma mensagem específica.</span><span class="sxs-lookup"><span data-stu-id="0d757-111">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="0d757-112">Esse mecanismo de deixar um aplicativo para definir e obter menções nas mensagens habilita notificações de leve, onde o usuário que está fazendo a mencionam pode permanecer no contexto existente (por exemplo, redigir um corpo de mensagem) enquanto o aplicativo define a propriedade subjacente **menções** .</span><span class="sxs-lookup"><span data-stu-id="0d757-112">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="0d757-113">Mencionado pessoas facilmente podem descobrir se e onde eles são mencionados por meio de `GET` solicitações com o `$filter` ou `$expand` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="0d757-113">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="0d757-114">Por exemplo, no cliente de email do Outlook, quando um usuário digita `@` ao escrever uma mensagem, o Outlook permite que o usuário selecione ou digite um nome para concluir o @-mencionam.</span><span class="sxs-lookup"><span data-stu-id="0d757-114">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="0d757-115">Outlook define a propriedade **menções** antes que ele cria e envia a mensagem ou evento.</span><span class="sxs-lookup"><span data-stu-id="0d757-115">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="0d757-116">O Outlook também usa `GET` operações com `$filter` e `$expand` para permitir que o usuário entrou no procurar mensagens que mencionar o usuário, alertando o usuário para itens de ação ou discussões, que permite uma resposta mais rápida.</span><span class="sxs-lookup"><span data-stu-id="0d757-116">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0d757-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d757-117">JSON representation</span></span>

<span data-ttu-id="0d757-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d757-118">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0d757-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d757-119">Properties</span></span>
| <span data-ttu-id="0d757-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d757-120">Property</span></span>     | <span data-ttu-id="0d757-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d757-121">Type</span></span>   |<span data-ttu-id="0d757-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d757-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d757-123">aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d757-123">application</span></span> | <span data-ttu-id="0d757-124">String</span><span class="sxs-lookup"><span data-stu-id="0d757-124">String</span></span> | <span data-ttu-id="0d757-125">O nome do aplicativo onde o mencionam é criado.</span><span class="sxs-lookup"><span data-stu-id="0d757-125">The name of the application where the mention is created.</span></span> <span data-ttu-id="0d757-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0d757-126">Optional.</span></span> <span data-ttu-id="0d757-127">Não é usado e o padrão como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="0d757-127">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="0d757-128">clientReference</span><span class="sxs-lookup"><span data-stu-id="0d757-128">clientReference</span></span> | <span data-ttu-id="0d757-129">String</span><span class="sxs-lookup"><span data-stu-id="0d757-129">String</span></span> | <span data-ttu-id="0d757-130">Um identificador exclusivo que representa um pai da instância do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d757-130">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="0d757-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0d757-131">Optional.</span></span> <span data-ttu-id="0d757-132">Não é usado e o padrão como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="0d757-132">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="0d757-133">createdBy</span><span class="sxs-lookup"><span data-stu-id="0d757-133">createdBy</span></span>  | [<span data-ttu-id="0d757-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0d757-134">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="0d757-135">As informações de email do usuário que fez a mencionam.</span><span class="sxs-lookup"><span data-stu-id="0d757-135">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="0d757-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d757-136">createdDateTime</span></span>  |<span data-ttu-id="0d757-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d757-137">DateTimeOffset</span></span> |<span data-ttu-id="0d757-138">A data e hora em que o mencionam é criado no cliente.</span><span class="sxs-lookup"><span data-stu-id="0d757-138">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="0d757-139">deepLink</span><span class="sxs-lookup"><span data-stu-id="0d757-139">deepLink</span></span> | <span data-ttu-id="0d757-140">String</span><span class="sxs-lookup"><span data-stu-id="0d757-140">String</span></span> | <span data-ttu-id="0d757-141">Um link profundo web ao contexto do mencionam na instância do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d757-141">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="0d757-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0d757-142">Optional.</span></span> <span data-ttu-id="0d757-143">Não é usado e o padrão como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="0d757-143">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="0d757-144">id</span><span class="sxs-lookup"><span data-stu-id="0d757-144">id</span></span> | <span data-ttu-id="0d757-145">String</span><span class="sxs-lookup"><span data-stu-id="0d757-145">String</span></span>| <span data-ttu-id="0d757-146">O identificador exclusivo de um mencionam em uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="0d757-146">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="0d757-147">mencionado</span><span class="sxs-lookup"><span data-stu-id="0d757-147">mentioned</span></span> | [<span data-ttu-id="0d757-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0d757-148">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="0d757-149">As informações de email da pessoa mencionada.</span><span class="sxs-lookup"><span data-stu-id="0d757-149">The email information of the mentioned person.</span></span> <span data-ttu-id="0d757-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d757-150">Required.</span></span> |
|<span data-ttu-id="0d757-151">mentionText</span><span class="sxs-lookup"><span data-stu-id="0d757-151">mentionText</span></span> | <span data-ttu-id="0d757-152">String</span><span class="sxs-lookup"><span data-stu-id="0d757-152">String</span></span> | <span data-ttu-id="0d757-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0d757-153">Optional.</span></span> <span data-ttu-id="0d757-154">Não é usado e o padrão como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="0d757-154">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="0d757-155">Para obter as menções em uma mensagem, consulte a propriedade **bodyPreview** da mensagem em vez disso.</span><span class="sxs-lookup"><span data-stu-id="0d757-155">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="0d757-156">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d757-156">serverCreatedDateTime</span></span> | <span data-ttu-id="0d757-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d757-157">DateTimeOffset</span></span> | <span data-ttu-id="0d757-158">A data e hora em que o mencionam é criada no servidor.</span><span class="sxs-lookup"><span data-stu-id="0d757-158">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="0d757-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0d757-159">Optional.</span></span> <span data-ttu-id="0d757-160">Não é usado e o padrão como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="0d757-160">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0d757-161">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="0d757-161">Relationships</span></span>
<span data-ttu-id="0d757-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d757-162">None</span></span>


## <a name="methods"></a><span data-ttu-id="0d757-163">Métodos</span><span class="sxs-lookup"><span data-stu-id="0d757-163">Methods</span></span>

| <span data-ttu-id="0d757-164">Método</span><span class="sxs-lookup"><span data-stu-id="0d757-164">Method</span></span>           | <span data-ttu-id="0d757-165">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0d757-165">Return Type</span></span>    |<span data-ttu-id="0d757-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d757-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d757-167">[POST](../api/user-sendmail.md#request-2) e enviar</span><span class="sxs-lookup"><span data-stu-id="0d757-167">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="0d757-168">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d757-168">None</span></span> | <span data-ttu-id="0d757-169">Criar e enviar menções como parte de uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="0d757-169">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="0d757-170">[Post](../api/user-post-messages.md#request-2) para um novo rascunho</span><span class="sxs-lookup"><span data-stu-id="0d757-170">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="0d757-171">[mensagem](../resources/message.md) que contém um ou mais objetos **mencionar** .</span><span class="sxs-lookup"><span data-stu-id="0d757-171">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="0d757-172">Criar um rascunho de uma nova mensagem e incluir um ou mais objetos **mencionar** .</span><span class="sxs-lookup"><span data-stu-id="0d757-172">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="0d757-173">Mensagens de [obter](../api/user-list-messages.md#request-2) mencionar me</span><span class="sxs-lookup"><span data-stu-id="0d757-173">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="0d757-174">Coleção [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="0d757-174">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="0d757-175">Obtenha todas as mensagens na caixa de correio do usuário conectado que contêm um **mencionar** deste usuário.</span><span class="sxs-lookup"><span data-stu-id="0d757-175">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="0d757-176">[Obtenha](../api/message-get.md#request-2) uma mensagem e seus menções</span><span class="sxs-lookup"><span data-stu-id="0d757-176">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="0d757-177">Coleção [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="0d757-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="0d757-178">Obtenha uma mensagem e expanda os detalhes de cada **mencionar** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="0d757-178">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="0d757-179">Excluir uma menção</span><span class="sxs-lookup"><span data-stu-id="0d757-179">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="0d757-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d757-180">None</span></span> |<span data-ttu-id="0d757-181">Exclui a menção especificada na mensagem especificada na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="0d757-181">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
