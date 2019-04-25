---
title: tipo de recurso menção
description: Representa uma notificação para uma pessoa com base no endereço de email da pessoa.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8e04722edf878b4f3851de837908dc5c0a02de7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523469"
---
# <a name="mention-resource-type"></a><span data-ttu-id="89efc-103">tipo de recurso menção</span><span class="sxs-lookup"><span data-stu-id="89efc-103">mention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89efc-104">Representa uma notificação para uma pessoa com base no endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="89efc-104">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="89efc-105">Esse tipo de notificação também é conhecido como @ menciona.</span><span class="sxs-lookup"><span data-stu-id="89efc-105">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="89efc-106">O recurso [Message](../resources/message.md) dá suporte a **menção**.</span><span class="sxs-lookup"><span data-stu-id="89efc-106">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="89efc-107">Ele inclui uma propriedade **mentionsPreview** que indica se o usuário conectado é mencionado nessa instância de mensagem.</span><span class="sxs-lookup"><span data-stu-id="89efc-107">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="89efc-108">Ele também inclui a propriedade de navegação **menciona** , que oferece suporte a obter detalhes de uma menção ou excluir uma menção nessa instância.</span><span class="sxs-lookup"><span data-stu-id="89efc-108">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="89efc-109">Ao criar uma mensagem, um aplicativo pode criar uma menção na mesma `POST` solicitação, incluindo a menção na propriedade **menciona** .</span><span class="sxs-lookup"><span data-stu-id="89efc-109">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="89efc-110">Usando uma `GET` solicitação com o `$filter` parâmetro de consulta, um aplicativo pode retornar todas as mensagens na caixa de correio do usuário conectado que mencionam o usuário.</span><span class="sxs-lookup"><span data-stu-id="89efc-110">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="89efc-111">Uma `GET` solicitação com o `$expand` parâmetro de consulta permite que o aplicativo expanda todas as menção em uma mensagem específica.</span><span class="sxs-lookup"><span data-stu-id="89efc-111">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="89efc-112">Esse mecanismo de permitir que um aplicativo defina e receba mençãos em mensagens permite notificações leves, em que o usuário que faz a menção pode permanecer no contexto existente (como compor um corpo de mensagem) enquanto o aplicativo define \*\*\*\* a propriedade mençãos subjacentes .</span><span class="sxs-lookup"><span data-stu-id="89efc-112">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="89efc-113">As pessoas mencionadas podem descobrir facilmente se e onde são mencionadas `GET` por meio de `$filter` solicitações `$expand` com o parâmetro ou consulta.</span><span class="sxs-lookup"><span data-stu-id="89efc-113">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="89efc-114">Por exemplo, no cliente de email do Outlook, quando um usuário `@` digita uma mensagem, o Outlook permite que o usuário selecione ou insira um nome para concluir a menção @.</span><span class="sxs-lookup"><span data-stu-id="89efc-114">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="89efc-115">O Outlook define a propriedade **menciona** antes de criar e enviar a mensagem ou o evento.</span><span class="sxs-lookup"><span data-stu-id="89efc-115">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="89efc-116">O Outlook também `GET` usa operações `$filter` com `$expand` o e para permitir que o usuário conectado procure mensagens que mencionam o usuário, alertando o usuário sobre itens de ação ou discussões, o que permite uma resposta mais rápida.</span><span class="sxs-lookup"><span data-stu-id="89efc-116">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="89efc-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89efc-117">JSON representation</span></span>

<span data-ttu-id="89efc-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89efc-118">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="89efc-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89efc-119">Properties</span></span>
| <span data-ttu-id="89efc-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89efc-120">Property</span></span>     | <span data-ttu-id="89efc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="89efc-121">Type</span></span>   |<span data-ttu-id="89efc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="89efc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89efc-123">application</span><span class="sxs-lookup"><span data-stu-id="89efc-123">application</span></span> | <span data-ttu-id="89efc-124">String</span><span class="sxs-lookup"><span data-stu-id="89efc-124">String</span></span> | <span data-ttu-id="89efc-125">O nome do aplicativo em que a menção é criada.</span><span class="sxs-lookup"><span data-stu-id="89efc-125">The name of the application where the mention is created.</span></span> <span data-ttu-id="89efc-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="89efc-126">Optional.</span></span> <span data-ttu-id="89efc-127">Não usado e padronizado como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="89efc-127">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="89efc-128">clientReference</span><span class="sxs-lookup"><span data-stu-id="89efc-128">clientReference</span></span> | <span data-ttu-id="89efc-129">String</span><span class="sxs-lookup"><span data-stu-id="89efc-129">String</span></span> | <span data-ttu-id="89efc-130">Um identificador exclusivo que representa um pai da instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="89efc-130">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="89efc-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="89efc-131">Optional.</span></span> <span data-ttu-id="89efc-132">Não usado e padronizado como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="89efc-132">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="89efc-133">createdBy</span><span class="sxs-lookup"><span data-stu-id="89efc-133">createdBy</span></span>  | [<span data-ttu-id="89efc-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="89efc-134">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="89efc-135">As informações de email do usuário que fez a menção.</span><span class="sxs-lookup"><span data-stu-id="89efc-135">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="89efc-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89efc-136">createdDateTime</span></span>  |<span data-ttu-id="89efc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89efc-137">DateTimeOffset</span></span> |<span data-ttu-id="89efc-138">A data e a hora em que a menção é criada no cliente.</span><span class="sxs-lookup"><span data-stu-id="89efc-138">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="89efc-139">deepLink</span><span class="sxs-lookup"><span data-stu-id="89efc-139">deepLink</span></span> | <span data-ttu-id="89efc-140">String</span><span class="sxs-lookup"><span data-stu-id="89efc-140">String</span></span> | <span data-ttu-id="89efc-141">Um link profundo da Web para o contexto de menção na instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="89efc-141">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="89efc-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="89efc-142">Optional.</span></span> <span data-ttu-id="89efc-143">Não usado e padronizado como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="89efc-143">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="89efc-144">id</span><span class="sxs-lookup"><span data-stu-id="89efc-144">id</span></span> | <span data-ttu-id="89efc-145">String</span><span class="sxs-lookup"><span data-stu-id="89efc-145">String</span></span>| <span data-ttu-id="89efc-146">O identificador exclusivo de uma menção em uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="89efc-146">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="89efc-147">foi</span><span class="sxs-lookup"><span data-stu-id="89efc-147">mentioned</span></span> | [<span data-ttu-id="89efc-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="89efc-148">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="89efc-149">As informações de email da pessoa mencionada.</span><span class="sxs-lookup"><span data-stu-id="89efc-149">The email information of the mentioned person.</span></span> <span data-ttu-id="89efc-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89efc-150">Required.</span></span> |
|<span data-ttu-id="89efc-151">mentionText</span><span class="sxs-lookup"><span data-stu-id="89efc-151">mentionText</span></span> | <span data-ttu-id="89efc-152">String</span><span class="sxs-lookup"><span data-stu-id="89efc-152">String</span></span> | <span data-ttu-id="89efc-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="89efc-153">Optional.</span></span> <span data-ttu-id="89efc-154">Não usado e padronizado como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="89efc-154">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="89efc-155">Para obter as menção em uma mensagem, confira a propriedade **bodyPreview** da mensagem.</span><span class="sxs-lookup"><span data-stu-id="89efc-155">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="89efc-156">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="89efc-156">serverCreatedDateTime</span></span> | <span data-ttu-id="89efc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89efc-157">DateTimeOffset</span></span> | <span data-ttu-id="89efc-158">A data e a hora em que a menção é criada no servidor.</span><span class="sxs-lookup"><span data-stu-id="89efc-158">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="89efc-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="89efc-159">Optional.</span></span> <span data-ttu-id="89efc-160">Não usado e padronizado como nulo para a **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="89efc-160">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="89efc-161">Relações</span><span class="sxs-lookup"><span data-stu-id="89efc-161">Relationships</span></span>
<span data-ttu-id="89efc-162">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="89efc-162">None</span></span>


## <a name="methods"></a><span data-ttu-id="89efc-163">Métodos</span><span class="sxs-lookup"><span data-stu-id="89efc-163">Methods</span></span>

| <span data-ttu-id="89efc-164">Método</span><span class="sxs-lookup"><span data-stu-id="89efc-164">Method</span></span>           | <span data-ttu-id="89efc-165">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="89efc-165">Return Type</span></span>    |<span data-ttu-id="89efc-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="89efc-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89efc-167">[Post](../api/user-sendmail.md#request-2) e Send</span><span class="sxs-lookup"><span data-stu-id="89efc-167">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="89efc-168">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89efc-168">None</span></span> | <span data-ttu-id="89efc-169">Criar e enviar mençãos como parte de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="89efc-169">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="89efc-170">[Postar](../api/user-post-messages.md#request-2) em um novo rascunho</span><span class="sxs-lookup"><span data-stu-id="89efc-170">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="89efc-171">[mensagem](../resources/message.md) que contém um ou mais objetos de **menção** .</span><span class="sxs-lookup"><span data-stu-id="89efc-171">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="89efc-172">Crie um rascunho de uma nova mensagem e inclua um ou mais objetos de **menção** .</span><span class="sxs-lookup"><span data-stu-id="89efc-172">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="89efc-173">[Obter](../api/user-list-messages.md#request-2) mensagens mencionando-me</span><span class="sxs-lookup"><span data-stu-id="89efc-173">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="89efc-174">Coleção [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="89efc-174">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="89efc-175">Obtenha todas as mensagens na caixa de correio do usuário conectado que contenham **menção** deste usuário.</span><span class="sxs-lookup"><span data-stu-id="89efc-175">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="89efc-176">[Obter](../api/message-get.md#request-2) uma mensagem e suas mencionações</span><span class="sxs-lookup"><span data-stu-id="89efc-176">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="89efc-177">Coleção [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="89efc-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="89efc-178">Obtenha uma mensagem e expanda os detalhes de cada **menção** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="89efc-178">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="89efc-179">[Excluir](../api/message-delete.md#request-2) uma menção</span><span class="sxs-lookup"><span data-stu-id="89efc-179">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="89efc-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89efc-180">None</span></span> |<span data-ttu-id="89efc-181">Exclui a menção especificada na mensagem especificada na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="89efc-181">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

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
