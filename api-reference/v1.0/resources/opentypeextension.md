---
title: Tipo de recurso openTypeExtension (extensões abertas)
description: As extensões abertas (anteriormente conhecidas como extensões de dados do Office 365) oferecem uma maneira fácil de adicionar diretamente propriedades não tipadas a um recurso do Microsoft Graph.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: fae3e9d791f74951cea2a1a4b2ed5ebd654b374e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730294"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="413bb-103">Tipo de recurso openTypeExtension (extensões abertas)</span><span class="sxs-lookup"><span data-stu-id="413bb-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="413bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="413bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="413bb-105">As extensões abertas (anteriormente conhecidas como extensões de dados do Office 365) oferecem uma maneira fácil de adicionar diretamente propriedades não tipadas a um recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="413bb-105">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="413bb-106">Extensões abertas são representadas pelo recurso **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="413bb-106">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="413bb-107">Qualquer extensão aberta adicionada a um recurso é mostrada na propriedade de navegação **extensions**, que deriva do tipo abstrato [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="413bb-107">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="413bb-108">Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="413bb-108">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="413bb-109">Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="413bb-109">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="413bb-110">Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.</span><span class="sxs-lookup"><span data-stu-id="413bb-110">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="413bb-111">Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="413bb-111">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="413bb-112">As extensões abertas têm suporte nos recursos a seguir nas versões correspondentes - disponibilidade geral (GA: /v1.0 e /beta) ou visualização (/beta).</span><span class="sxs-lookup"><span data-stu-id="413bb-112">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="413bb-113">Recurso</span><span class="sxs-lookup"><span data-stu-id="413bb-113">Resource</span></span> |<span data-ttu-id="413bb-114">Versão</span><span class="sxs-lookup"><span data-stu-id="413bb-114">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="413bb-115">Unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="413bb-115">Administrative unit</span></span>](/graph/api/resources/administrativeunit?view=graph-rest-beta)  | <span data-ttu-id="413bb-116">Somente para visualização</span><span class="sxs-lookup"><span data-stu-id="413bb-116">Preview only</span></span> |
| [<span data-ttu-id="413bb-117">Evento de calendário</span><span class="sxs-lookup"><span data-stu-id="413bb-117">Calendar event</span></span>](event.md) | <span data-ttu-id="413bb-118">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-118">GA</span></span> |
| <span data-ttu-id="413bb-119">[Evento de calendário](event.md) do grupo</span><span class="sxs-lookup"><span data-stu-id="413bb-119">Group [calendar event](event.md)</span></span> | <span data-ttu-id="413bb-120">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-120">GA</span></span> |
| <span data-ttu-id="413bb-121">[Postagem](post.md) de thread de conversa do grupo</span><span class="sxs-lookup"><span data-stu-id="413bb-121">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="413bb-122">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-122">GA</span></span> |
| [<span data-ttu-id="413bb-123">device</span><span class="sxs-lookup"><span data-stu-id="413bb-123">device</span></span>](device.md) | <span data-ttu-id="413bb-124">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-124">GA</span></span> |
| [<span data-ttu-id="413bb-125">group</span><span class="sxs-lookup"><span data-stu-id="413bb-125">group</span></span>](group.md) | <span data-ttu-id="413bb-126">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-126">GA</span></span> |
| [<span data-ttu-id="413bb-127">message</span><span class="sxs-lookup"><span data-stu-id="413bb-127">message</span></span>](message.md) | <span data-ttu-id="413bb-128">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-128">GA</span></span> |
| [<span data-ttu-id="413bb-129">organization</span><span class="sxs-lookup"><span data-stu-id="413bb-129">organization</span></span>](organization.md) | <span data-ttu-id="413bb-130">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-130">GA</span></span> |
| [<span data-ttu-id="413bb-131">Contato pessoal</span><span class="sxs-lookup"><span data-stu-id="413bb-131">Personal contact</span></span>](contact.md) | <span data-ttu-id="413bb-132">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-132">GA</span></span> |
| [<span data-ttu-id="413bb-133">user</span><span class="sxs-lookup"><span data-stu-id="413bb-133">user</span></span>](user.md) | <span data-ttu-id="413bb-134">GA</span><span class="sxs-lookup"><span data-stu-id="413bb-134">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="413bb-135">Considerações específicas do Outlook</span><span class="sxs-lookup"><span data-stu-id="413bb-135">Outlook-specific considerations</span></span>

<span data-ttu-id="413bb-136">Cada extensão aberta presente em um recurso do Outlook (evento, mensagem ou contato pessoal) é armazenada em uma [propriedade MAPI](/office/client-developer/outlook/mapi/mapi-named-properties).</span><span class="sxs-lookup"><span data-stu-id="413bb-136">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](/office/client-developer/outlook/mapi/mapi-named-properties).</span></span> <span data-ttu-id="413bb-137">Quando você cria extensões abertas no Outlook, considere que as propriedades MAPI são um recurso finito em uma caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="413bb-137">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="413bb-138">Quando a propriedade de cota de um usuário acabar, não será mais possível criar quaisquer propriedades nomeadas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="413bb-138">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="413bb-139">Isso pode resultar em um comportamento inesperado de clientes que dependem de propriedades nomeadas para funcionar.</span><span class="sxs-lookup"><span data-stu-id="413bb-139">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="413bb-140">Aplique as seguintes diretrizes quando você criar extensões abertas em recursos do Outlook:</span><span class="sxs-lookup"><span data-stu-id="413bb-140">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="413bb-141">Crie um número mínimo de extensões necessárias.</span><span class="sxs-lookup"><span data-stu-id="413bb-141">Create the minimum number of extensions required.</span></span> <span data-ttu-id="413bb-142">A maioria dos aplicativos exigem não mais que uma extensão.</span><span class="sxs-lookup"><span data-stu-id="413bb-142">Most applications should require no more than one extension.</span></span> <span data-ttu-id="413bb-143">As extensões não têm um conjunto definido de propriedades nomeadas ou estrutura, para que seja possível armazenar vários valores em um única extensão.</span><span class="sxs-lookup"><span data-stu-id="413bb-143">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="413bb-144">Evite renomear extensões de uma maneira variável (por exemplo, com base na entrada do usuário, etc.).</span><span class="sxs-lookup"><span data-stu-id="413bb-144">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="413bb-145">Sempre que uma extensão aberta é criada com um novo nome que não foi usado na caixa de correio do usuário, uma nova propriedade MAPI é criada.</span><span class="sxs-lookup"><span data-stu-id="413bb-145">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="413bb-146">Remover a extensão não remove a propriedade nomeada.</span><span class="sxs-lookup"><span data-stu-id="413bb-146">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="413bb-147">Use extensões abertas (para recursos do Outlook) ou propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="413bb-147">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="413bb-148">Extensões abertas são a solução recomendada para a maioria dos cenários que envolvem armazenar e acessar dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="413bb-148">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="413bb-149">Se, no entanto, você precisar acessar dados personalizados para as propriedades do Outlook MAPI que já não estão expostos por meio dos [metadados da API do Microsoft Graph](../index.md), você pode usar [as propriedades estendidas e sua API REST](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="413bb-149">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](../index.md), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="413bb-150">Você pode verificar quais propriedades os metadados expõem na [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="413bb-150">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="413bb-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="413bb-151">JSON representation</span></span>

<span data-ttu-id="413bb-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="413bb-152">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="413bb-153">Propriedades</span><span class="sxs-lookup"><span data-stu-id="413bb-153">Properties</span></span>

|<span data-ttu-id="413bb-154">Propriedade</span><span class="sxs-lookup"><span data-stu-id="413bb-154">Property</span></span> | <span data-ttu-id="413bb-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="413bb-155">Type</span></span> | <span data-ttu-id="413bb-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="413bb-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="413bb-157">extensionName</span><span class="sxs-lookup"><span data-stu-id="413bb-157">extensionName</span></span>|<span data-ttu-id="413bb-158">String</span><span class="sxs-lookup"><span data-stu-id="413bb-158">String</span></span>|<span data-ttu-id="413bb-p107">Um identificador de texto exclusivo para uma extensão de tipo aberto. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="413bb-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="413bb-161">id</span><span class="sxs-lookup"><span data-stu-id="413bb-161">id</span></span>|<span data-ttu-id="413bb-162">String</span><span class="sxs-lookup"><span data-stu-id="413bb-162">String</span></span>| <span data-ttu-id="413bb-p108">Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="413bb-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="413bb-165">Relações</span><span class="sxs-lookup"><span data-stu-id="413bb-165">Relationships</span></span>

<span data-ttu-id="413bb-166">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="413bb-166">None</span></span>

## <a name="methods"></a><span data-ttu-id="413bb-167">Métodos</span><span class="sxs-lookup"><span data-stu-id="413bb-167">Methods</span></span>

|<span data-ttu-id="413bb-168">Método</span><span class="sxs-lookup"><span data-stu-id="413bb-168">Method</span></span> | <span data-ttu-id="413bb-169">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="413bb-169">Return Type</span></span> | <span data-ttu-id="413bb-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="413bb-170">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="413bb-171">Criar</span><span class="sxs-lookup"><span data-stu-id="413bb-171">Create</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="413bb-172">[openTypeExtension](opentypeextension.md) (em uma instância de recurso existente) ou um novo [contact](../resources/contact.md), [event](../resources/event.md) ou [message](../resources/message.md) que contenha um objeto openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="413bb-172">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="413bb-173">Crie um objeto openTypeExtension em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="413bb-173">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="413bb-174">Get</span><span class="sxs-lookup"><span data-stu-id="413bb-174">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="413bb-175">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="413bb-175">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="413bb-176">Leia propriedades e relações do objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="413bb-176">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="413bb-177">Update</span><span class="sxs-lookup"><span data-stu-id="413bb-177">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="413bb-178">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="413bb-178">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="413bb-179">Atualize o objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="413bb-179">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="413bb-180">Delete</span><span class="sxs-lookup"><span data-stu-id="413bb-180">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="413bb-181">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="413bb-181">None</span></span> |<span data-ttu-id="413bb-182">Exclua um objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="413bb-182">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
