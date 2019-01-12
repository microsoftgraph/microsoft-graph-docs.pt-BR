---
title: Tipo de recurso openTypeExtension (extensões abertas)
description: Extensões de Open (conhecidas anteriormente como extensões de dados do Office 365) fornecem uma maneira fácil de adicionar diretamente sem tipo propriedades para um recurso no Microsoft Graph.
localization_priority: Priority
author: dkershaw10
ms.openlocfilehash: 854897e1cc4d887fc0f4d2f184a4e745e5cdc468
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977511"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="6e449-103">Tipo de recurso openTypeExtension (extensões abertas)</span><span class="sxs-lookup"><span data-stu-id="6e449-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="6e449-104">Extensões de Open (conhecidas anteriormente como extensões de dados do Office 365) fornecem uma maneira fácil de adicionar diretamente sem tipo propriedades para um recurso no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6e449-104">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="6e449-105">Extensões abertas são representadas pelo recurso **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="6e449-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="6e449-106">Qualquer extensão aberta adicionada a um recurso é mostrada na propriedade de navegação **extensions**, que deriva do tipo abstrato [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="6e449-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="6e449-107">Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="6e449-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="6e449-108">Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="6e449-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="6e449-109">Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.</span><span class="sxs-lookup"><span data-stu-id="6e449-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="6e449-110">Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="6e449-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="6e449-111">As extensões abertas têm suporte nos recursos a seguir nas versões correspondentes - disponibilidade geral (GA: /v1.0 e /beta) ou visualização (/beta).</span><span class="sxs-lookup"><span data-stu-id="6e449-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="6e449-112">Recurso</span><span class="sxs-lookup"><span data-stu-id="6e449-112">Resource</span></span> |<span data-ttu-id="6e449-113">Versão</span><span class="sxs-lookup"><span data-stu-id="6e449-113">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="6e449-114">Unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="6e449-114">Administrative unit</span></span>](/graph/api/resources/administrativeunit?view=graph-rest-beta)  | <span data-ttu-id="6e449-115">Somente para visualização</span><span class="sxs-lookup"><span data-stu-id="6e449-115">Preview only</span></span> |
| [<span data-ttu-id="6e449-116">Evento de calendário</span><span class="sxs-lookup"><span data-stu-id="6e449-116">Calendar event</span></span>](event.md) | <span data-ttu-id="6e449-117">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-117">GA</span></span> |
| <span data-ttu-id="6e449-118">[Evento de calendário](event.md) do grupo</span><span class="sxs-lookup"><span data-stu-id="6e449-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="6e449-119">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-119">GA</span></span> |
| <span data-ttu-id="6e449-120">[Postagem](post.md) de thread de conversa do grupo</span><span class="sxs-lookup"><span data-stu-id="6e449-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="6e449-121">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-121">GA</span></span> |
| [<span data-ttu-id="6e449-122">device</span><span class="sxs-lookup"><span data-stu-id="6e449-122">device</span></span>](device.md) | <span data-ttu-id="6e449-123">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-123">GA</span></span> |
| [<span data-ttu-id="6e449-124">group</span><span class="sxs-lookup"><span data-stu-id="6e449-124">group</span></span>](group.md) | <span data-ttu-id="6e449-125">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-125">GA</span></span> |
| [<span data-ttu-id="6e449-126">message</span><span class="sxs-lookup"><span data-stu-id="6e449-126">message</span></span>](message.md) | <span data-ttu-id="6e449-127">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-127">GA</span></span> |
| [<span data-ttu-id="6e449-128">organization</span><span class="sxs-lookup"><span data-stu-id="6e449-128">organization</span></span>](organization.md) | <span data-ttu-id="6e449-129">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-129">GA</span></span> |
| [<span data-ttu-id="6e449-130">Contato pessoal</span><span class="sxs-lookup"><span data-stu-id="6e449-130">Personal contact</span></span>](contact.md) | <span data-ttu-id="6e449-131">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-131">GA</span></span> |
| [<span data-ttu-id="6e449-132">user</span><span class="sxs-lookup"><span data-stu-id="6e449-132">user</span></span>](user.md) | <span data-ttu-id="6e449-133">GA</span><span class="sxs-lookup"><span data-stu-id="6e449-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="6e449-134">Considerações específicas do Outlook</span><span class="sxs-lookup"><span data-stu-id="6e449-134">Outlook-specific considerations</span></span>

<span data-ttu-id="6e449-135">Cada extensão aberta presente em um recurso do Outlook (evento, mensagem ou contato pessoal) é armazenado em uma [propriedade MAPI nomeada](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span><span class="sxs-lookup"><span data-stu-id="6e449-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="6e449-136">Quando você cria extensões abertas para o Outlook, considere que o MAPI denominada propriedades sejam um recurso finito na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="6e449-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="6e449-137">Quando for esgotada cota do nome da propriedade de um usuário, é possível criar qualquer propriedades nomeadas mais para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="6e449-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="6e449-138">Isso pode resultar em um comportamento inesperado de clientes que dependem de propriedades nomeadas funcione.</span><span class="sxs-lookup"><span data-stu-id="6e449-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="6e449-139">Aplique as seguintes diretrizes ao criar extensões open nos recursos do Outlook:</span><span class="sxs-lookup"><span data-stu-id="6e449-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="6e449-140">Crie o número mínimo de extensões necessárias.</span><span class="sxs-lookup"><span data-stu-id="6e449-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="6e449-141">A maioria dos aplicativos deve exigir que não mais de uma extensão.</span><span class="sxs-lookup"><span data-stu-id="6e449-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="6e449-142">As extensões não têm propriedades de conjunto definido ou estrutura, permitindo que você armazene vários valores em um única extensão.</span><span class="sxs-lookup"><span data-stu-id="6e449-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="6e449-143">Evite extensões de nomes de maneira variável (como com base na entrada do usuário, etc.).</span><span class="sxs-lookup"><span data-stu-id="6e449-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="6e449-144">Cada vez que uma extensão aberta é criada com um novo nome não tiver sido usado na caixa de correio de um usuário antes, um novo MAPI denominado propriedade é criado.</span><span class="sxs-lookup"><span data-stu-id="6e449-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="6e449-145">Removendo a extensão não remove a propriedade nomeada.</span><span class="sxs-lookup"><span data-stu-id="6e449-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="6e449-146">Usar extensões open (para recursos do Outlook) ou propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="6e449-146">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="6e449-147">Extensões Open são a solução recomendada para a maioria dos cenários que envolvem armazenar e acessar dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="6e449-147">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="6e449-148">Se, no entanto, você precisar acessar dados personalizados para propriedades MAPI do Outlook que não são expostos por meio de [metadados de API do Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api), você pode usar [propriedades estendidas e seus API REST](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="6e449-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="6e449-149">Você pode verificar quais propriedades os metadados expõe em [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="6e449-149">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e449-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e449-150">JSON representation</span></span>

<span data-ttu-id="6e449-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e449-151">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a><span data-ttu-id="6e449-152">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e449-152">Properties</span></span>

|<span data-ttu-id="6e449-153">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e449-153">Property</span></span> | <span data-ttu-id="6e449-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e449-154">Type</span></span> | <span data-ttu-id="6e449-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e449-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6e449-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="6e449-156">extensionName</span></span>|<span data-ttu-id="6e449-157">String</span><span class="sxs-lookup"><span data-stu-id="6e449-157">String</span></span>|<span data-ttu-id="6e449-p107">Um identificador de texto exclusivo para uma extensão de tipo aberto. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e449-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="6e449-160">id</span><span class="sxs-lookup"><span data-stu-id="6e449-160">id</span></span>|<span data-ttu-id="6e449-161">String</span><span class="sxs-lookup"><span data-stu-id="6e449-161">String</span></span>| <span data-ttu-id="6e449-p108">Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e449-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e449-164">Relações</span><span class="sxs-lookup"><span data-stu-id="6e449-164">Relationships</span></span>

<span data-ttu-id="6e449-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e449-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="6e449-166">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e449-166">Methods</span></span>

|<span data-ttu-id="6e449-167">Método</span><span class="sxs-lookup"><span data-stu-id="6e449-167">Method</span></span> | <span data-ttu-id="6e449-168">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e449-168">Return Type</span></span> | <span data-ttu-id="6e449-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e449-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e449-170">Post</span><span class="sxs-lookup"><span data-stu-id="6e449-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="6e449-171">[openTypeExtension](opentypeextension.md) (em uma instância de recurso existente) ou um novo [contact](../resources/contact.md), [event](../resources/event.md) ou [message](../resources/message.md) que contenha um objeto openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6e449-171">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="6e449-172">Crie um objeto openTypeExtension em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="6e449-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="6e449-173">Get</span><span class="sxs-lookup"><span data-stu-id="6e449-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="6e449-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6e449-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="6e449-175">Leia propriedades e relações do objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="6e449-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="6e449-176">Update</span><span class="sxs-lookup"><span data-stu-id="6e449-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="6e449-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6e449-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="6e449-178">Atualize o objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="6e449-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="6e449-179">Delete</span><span class="sxs-lookup"><span data-stu-id="6e449-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="6e449-180">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6e449-180">None</span></span> |<span data-ttu-id="6e449-181">Exclua um objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="6e449-181">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
