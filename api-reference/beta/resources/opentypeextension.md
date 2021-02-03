---
title: Tipo de recurso openTypeExtension (extensões abertas)
description: As extensões abertas (anteriormente conhecidas como extensões de dados do Office 365) oferecem uma maneira fácil de adicionar diretamente propriedades não tipadas a um recurso do Microsoft Graph.
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 4373bd4dcc911f08504e9716b1cc19d8d177df16
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092670"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="886fa-103">Tipo de recurso openTypeExtension (extensões abertas)</span><span class="sxs-lookup"><span data-stu-id="886fa-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="886fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="886fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="886fa-105">As extensões abertas (anteriormente conhecidas como extensões de dados do Office 365) oferecem uma maneira fácil de adicionar diretamente propriedades não tipadas a um recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="886fa-105">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="886fa-106">Extensões abertas são representadas pelo recurso **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="886fa-106">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="886fa-107">Qualquer extensão aberta adicionada a um recurso é mostrada na propriedade de navegação **extensions**, que deriva do tipo abstrato [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="886fa-107">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="886fa-108">Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="886fa-108">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="886fa-109">Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="886fa-109">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="886fa-110">Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.</span><span class="sxs-lookup"><span data-stu-id="886fa-110">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="886fa-111">Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="886fa-111">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="886fa-112">As extensões abertas têm suporte nos recursos a seguir nas versões correspondentes - disponibilidade geral (GA: /v1.0 e /beta) ou visualização (/beta).</span><span class="sxs-lookup"><span data-stu-id="886fa-112">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="886fa-113">Recurso</span><span class="sxs-lookup"><span data-stu-id="886fa-113">Resource</span></span> | <span data-ttu-id="886fa-114">Versão</span><span class="sxs-lookup"><span data-stu-id="886fa-114">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="886fa-115">Unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="886fa-115">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="886fa-116">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-116">GA</span></span> |
| [<span data-ttu-id="886fa-117">Evento de calendário</span><span class="sxs-lookup"><span data-stu-id="886fa-117">Calendar event</span></span>](event.md) | <span data-ttu-id="886fa-118">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-118">GA</span></span> |
| <span data-ttu-id="886fa-119">[Evento de calendário](event.md) do grupo</span><span class="sxs-lookup"><span data-stu-id="886fa-119">Group [calendar event](event.md)</span></span> | <span data-ttu-id="886fa-120">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-120">GA</span></span> |
| <span data-ttu-id="886fa-121">[Postagem](post.md) de thread de conversa do grupo</span><span class="sxs-lookup"><span data-stu-id="886fa-121">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="886fa-122">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-122">GA</span></span> |
| [<span data-ttu-id="886fa-123">Dispositivo</span><span class="sxs-lookup"><span data-stu-id="886fa-123">Device</span></span>](device.md) | <span data-ttu-id="886fa-124">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-124">GA</span></span> |
| [<span data-ttu-id="886fa-125">Grupo</span><span class="sxs-lookup"><span data-stu-id="886fa-125">Group</span></span>](group.md) | <span data-ttu-id="886fa-126">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-126">GA</span></span> |
| [<span data-ttu-id="886fa-127">Mensagem</span><span class="sxs-lookup"><span data-stu-id="886fa-127">Message</span></span>](message.md) | <span data-ttu-id="886fa-128">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-128">GA</span></span> |
| [<span data-ttu-id="886fa-129">Organização</span><span class="sxs-lookup"><span data-stu-id="886fa-129">Organization</span></span>](organization.md) | <span data-ttu-id="886fa-130">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-130">GA</span></span> |
| [<span data-ttu-id="886fa-131">Contato pessoal</span><span class="sxs-lookup"><span data-stu-id="886fa-131">Personal contact</span></span>](contact.md) | <span data-ttu-id="886fa-132">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-132">GA</span></span> |
| [<span data-ttu-id="886fa-133">Usuário</span><span class="sxs-lookup"><span data-stu-id="886fa-133">User</span></span>](user.md) | <span data-ttu-id="886fa-134">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-134">GA</span></span> |
| [<span data-ttu-id="886fa-135">Tarefa</span><span class="sxs-lookup"><span data-stu-id="886fa-135">Task</span></span>](todotask.md)  | <span data-ttu-id="886fa-136">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-136">GA</span></span> ||
| [<span data-ttu-id="886fa-137">Lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="886fa-137">Task list</span></span>](todotasklist.md)  | <span data-ttu-id="886fa-138">GA</span><span class="sxs-lookup"><span data-stu-id="886fa-138">GA</span></span> ||

## <a name="outlook-specific-considerations"></a><span data-ttu-id="886fa-139">Considerações específicas do Outlook</span><span class="sxs-lookup"><span data-stu-id="886fa-139">Outlook-specific considerations</span></span>

<span data-ttu-id="886fa-140">Cada extensão aberta presente em um recurso do Outlook (evento, mensagem ou contato pessoal) é armazenada em uma [propriedade MAPI](/office/client-developer/outlook/mapi/mapi-named-properties).</span><span class="sxs-lookup"><span data-stu-id="886fa-140">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](/office/client-developer/outlook/mapi/mapi-named-properties).</span></span> <span data-ttu-id="886fa-141">Quando você cria extensões abertas no Outlook, considere que as propriedades MAPI são um recurso finito em uma caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="886fa-141">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="886fa-142">Quando a propriedade de cota de um usuário acabar, não será mais possível criar quaisquer propriedades nomeadas desse usuário.</span><span class="sxs-lookup"><span data-stu-id="886fa-142">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="886fa-143">Isso pode resultar em um comportamento inesperado de clientes que dependem de propriedades nomeadas para funcionar.</span><span class="sxs-lookup"><span data-stu-id="886fa-143">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="886fa-144">Aplique as seguintes diretrizes quando você criar extensões abertas em recursos do Outlook:</span><span class="sxs-lookup"><span data-stu-id="886fa-144">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="886fa-145">Crie um número mínimo de extensões necessárias.</span><span class="sxs-lookup"><span data-stu-id="886fa-145">Create the minimum number of extensions required.</span></span> <span data-ttu-id="886fa-146">A maioria dos aplicativos exigem não mais que uma extensão.</span><span class="sxs-lookup"><span data-stu-id="886fa-146">Most applications should require no more than one extension.</span></span> <span data-ttu-id="886fa-147">As extensões não têm um conjunto definido de propriedades nomeadas ou estrutura, para que seja possível armazenar vários valores em um única extensão.</span><span class="sxs-lookup"><span data-stu-id="886fa-147">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="886fa-148">Evite renomear extensões de uma maneira variável (por exemplo, com base na entrada do usuário, etc.).</span><span class="sxs-lookup"><span data-stu-id="886fa-148">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="886fa-149">Sempre que uma extensão aberta é criada com um novo nome que não foi usado na caixa de correio do usuário, uma nova propriedade MAPI é criada.</span><span class="sxs-lookup"><span data-stu-id="886fa-149">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="886fa-150">Remover a extensão não remove a propriedade nomeada.</span><span class="sxs-lookup"><span data-stu-id="886fa-150">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="886fa-151">Use extensões abertas (para recursos do Outlook) ou propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="886fa-151">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="886fa-152">Extensões abertas são a solução recomendada para a maioria dos cenários que envolvem armazenar e acessar dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="886fa-152">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="886fa-153">Se, no entanto, você precisar acessar dados personalizados para as propriedades do Outlook MAPI que já não estão expostos por meio dos [metadados da API do Microsoft Graph](../index.md), você pode usar [as propriedades estendidas e sua API REST](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="886fa-153">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](../index.md), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="886fa-154">Você pode verificar quais propriedades os metadados expõem na [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="886fa-154">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="886fa-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="886fa-155">JSON representation</span></span>

<span data-ttu-id="886fa-156">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="886fa-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}
```

## <a name="properties"></a><span data-ttu-id="886fa-157">Propriedades</span><span class="sxs-lookup"><span data-stu-id="886fa-157">Properties</span></span>

| <span data-ttu-id="886fa-158">Propriedade</span><span class="sxs-lookup"><span data-stu-id="886fa-158">Property</span></span> | <span data-ttu-id="886fa-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="886fa-159">Type</span></span> | <span data-ttu-id="886fa-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="886fa-160">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="886fa-161">extensionName</span><span class="sxs-lookup"><span data-stu-id="886fa-161">extensionName</span></span>|<span data-ttu-id="886fa-162">String</span><span class="sxs-lookup"><span data-stu-id="886fa-162">String</span></span>|<span data-ttu-id="886fa-p106">Um identificador de texto exclusivo para uma extensão de dados de tipo aberto. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="886fa-p106">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="886fa-165">id</span><span class="sxs-lookup"><span data-stu-id="886fa-165">id</span></span>|<span data-ttu-id="886fa-166">String</span><span class="sxs-lookup"><span data-stu-id="886fa-166">String</span></span>| <span data-ttu-id="886fa-p107">Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="886fa-p107">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="886fa-169">Relações</span><span class="sxs-lookup"><span data-stu-id="886fa-169">Relationships</span></span>

<span data-ttu-id="886fa-170">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="886fa-170">None</span></span>

## <a name="methods"></a><span data-ttu-id="886fa-171">Métodos</span><span class="sxs-lookup"><span data-stu-id="886fa-171">Methods</span></span>

| <span data-ttu-id="886fa-172">Método</span><span class="sxs-lookup"><span data-stu-id="886fa-172">Method</span></span> | <span data-ttu-id="886fa-173">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="886fa-173">Return Type</span></span> | <span data-ttu-id="886fa-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="886fa-174">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="886fa-175">Criar</span><span class="sxs-lookup"><span data-stu-id="886fa-175">Create</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="886fa-176">[openTypeExtension](opentypeextension.md)(em uma instância de recurso existente) ou um novo contato [,](contact.md) [evento](event.md) [,](message.md)mensagem , [postagem](post.md), [todoTask](todotask.md)ou [todoTaskList](todotasklist.md) que contém um objeto openTypeExtension .</span><span class="sxs-lookup"><span data-stu-id="886fa-176">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](contact.md), [event](event.md), [message](message.md), [post](post.md), [todoTask](todotask.md), or [todoTaskList](todotasklist.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="886fa-177">Crie um objeto openTypeExtension em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="886fa-177">Create an openTypeExtension object in an existing or new resource instance.</span></span>||[<span data-ttu-id="886fa-178">Get</span><span class="sxs-lookup"><span data-stu-id="886fa-178">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="886fa-179">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="886fa-179">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="886fa-180">Leia propriedades e relações do objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="886fa-180">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="886fa-181">Update</span><span class="sxs-lookup"><span data-stu-id="886fa-181">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="886fa-182">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="886fa-182">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="886fa-183">Atualize o objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="886fa-183">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="886fa-184">Delete</span><span class="sxs-lookup"><span data-stu-id="886fa-184">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="886fa-185">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="886fa-185">None</span></span> |<span data-ttu-id="886fa-186">Exclua um objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="886fa-186">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
