---
title: Tipo de recurso openTypeExtension (extensões abertas)
description: As extensões abertas (anteriormente conhecidas como extensões de dados do Office 365) fornecem uma maneira fácil de adicionar diretamente Propriedades não tipadas a um recurso no Microsoft Graph.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: ba5dbcd6c5ae1705ffe7e89ca6f529280d98adf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568881"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="9016e-103">Tipo de recurso openTypeExtension (extensões abertas)</span><span class="sxs-lookup"><span data-stu-id="9016e-103">openTypeExtension resource type (open extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9016e-104">As extensões abertas (anteriormente conhecidas como extensões de dados do Office 365) fornecem uma maneira fácil de adicionar diretamente Propriedades não tipadas a um recurso no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9016e-104">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="9016e-105">Extensões abertas são representadas pelo recurso **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="9016e-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="9016e-106">Qualquer extensão aberta adicionada a um recurso é mostrada na propriedade de navegação **extensions**, que deriva do tipo abstrato [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="9016e-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="9016e-107">Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="9016e-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="9016e-108">Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="9016e-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="9016e-109">Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.</span><span class="sxs-lookup"><span data-stu-id="9016e-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="9016e-110">Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="9016e-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="9016e-111">As extensões abertas têm suporte nos recursos a seguir nas versões correspondentes - disponibilidade geral (GA: /v1.0 e /beta) ou visualização (/beta).</span><span class="sxs-lookup"><span data-stu-id="9016e-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="9016e-112">Recurso</span><span class="sxs-lookup"><span data-stu-id="9016e-112">Resource</span></span> | <span data-ttu-id="9016e-113">Versão</span><span class="sxs-lookup"><span data-stu-id="9016e-113">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="9016e-114">Unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="9016e-114">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="9016e-115">Somente para visualização</span><span class="sxs-lookup"><span data-stu-id="9016e-115">Preview only</span></span> |
| [<span data-ttu-id="9016e-116">Evento de calendário</span><span class="sxs-lookup"><span data-stu-id="9016e-116">Calendar event</span></span>](event.md) | <span data-ttu-id="9016e-117">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-117">GA</span></span> |
| <span data-ttu-id="9016e-118">[Evento de calendário](event.md) do grupo</span><span class="sxs-lookup"><span data-stu-id="9016e-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="9016e-119">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-119">GA</span></span> |
| <span data-ttu-id="9016e-120">[Postagem](post.md) de thread de conversa do grupo</span><span class="sxs-lookup"><span data-stu-id="9016e-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="9016e-121">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-121">GA</span></span> |
| [<span data-ttu-id="9016e-122">device</span><span class="sxs-lookup"><span data-stu-id="9016e-122">device</span></span>](device.md) | <span data-ttu-id="9016e-123">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-123">GA</span></span> |
| [<span data-ttu-id="9016e-124">group</span><span class="sxs-lookup"><span data-stu-id="9016e-124">group</span></span>](group.md) | <span data-ttu-id="9016e-125">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-125">GA</span></span> |
| [<span data-ttu-id="9016e-126">message</span><span class="sxs-lookup"><span data-stu-id="9016e-126">message</span></span>](message.md) | <span data-ttu-id="9016e-127">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-127">GA</span></span> |
| [<span data-ttu-id="9016e-128">organization</span><span class="sxs-lookup"><span data-stu-id="9016e-128">organization</span></span>](organization.md) | <span data-ttu-id="9016e-129">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-129">GA</span></span> |
| [<span data-ttu-id="9016e-130">Contato pessoal</span><span class="sxs-lookup"><span data-stu-id="9016e-130">Personal contact</span></span>](contact.md) | <span data-ttu-id="9016e-131">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-131">GA</span></span> |
| [<span data-ttu-id="9016e-132">user</span><span class="sxs-lookup"><span data-stu-id="9016e-132">user</span></span>](user.md) | <span data-ttu-id="9016e-133">GA</span><span class="sxs-lookup"><span data-stu-id="9016e-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="9016e-134">Considerações específicas do Outlook</span><span class="sxs-lookup"><span data-stu-id="9016e-134">Outlook-specific considerations</span></span>

<span data-ttu-id="9016e-135">Cada extensão aberta presente em um recurso do Outlook (evento, mensagem ou contato pessoal) é armazenada em uma [propriedade nomeada MAPI](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span><span class="sxs-lookup"><span data-stu-id="9016e-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="9016e-136">Ao criar extensões abertas para o Outlook, considere que as propriedades nomeadas de MAPI são um recurso finito na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9016e-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="9016e-137">Quando a cota de propriedade nomeada de um usuário é esgotada, você não pode criar mais propriedades nomeadas para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="9016e-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="9016e-138">Isso pode resultar em um comportamento inesperado de clientes que dependem de propriedades nomeadas para funcionar.</span><span class="sxs-lookup"><span data-stu-id="9016e-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="9016e-139">Aplique as seguintes diretrizes ao criar extensões abertas em recursos do Outlook:</span><span class="sxs-lookup"><span data-stu-id="9016e-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="9016e-140">Crie o número mínimo de extensões necessárias.</span><span class="sxs-lookup"><span data-stu-id="9016e-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="9016e-141">A maioria dos aplicativos não deve exigir mais de uma extensão.</span><span class="sxs-lookup"><span data-stu-id="9016e-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="9016e-142">As extensões não têm propriedades ou estruturas definidas para que você possa armazenar vários valores em uma única extensão.</span><span class="sxs-lookup"><span data-stu-id="9016e-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="9016e-143">Evite nomes de extensões de forma variável (por exemplo, com base na entrada do usuário, etc.).</span><span class="sxs-lookup"><span data-stu-id="9016e-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="9016e-144">Sempre que uma extensão aberta é criada com um novo nome que não foi usado na caixa de correio de um usuário, uma nova propriedade nomeada MAPI é criada.</span><span class="sxs-lookup"><span data-stu-id="9016e-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="9016e-145">Remover a extensão não remove a propriedade nomeada.</span><span class="sxs-lookup"><span data-stu-id="9016e-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="9016e-146">Usar extensões abertas (para recursos do Outlook) ou propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="9016e-146">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="9016e-147">As extensões abertas são a solução recomendada para a maioria dos cenários que envolvem o armazenamento e o acesso a dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="9016e-147">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="9016e-148">Se, no entanto, você precisar acessar dados personalizados para as propriedades do Outlook MAPI que já não estão expostos por meio dos [metadados da API do Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api), você pode usar [as propriedades estendidas e sua API REST](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9016e-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="9016e-149">você pode verificar quais propriedades os metadados expões em [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="9016e-149">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9016e-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9016e-150">JSON representation</span></span>

<span data-ttu-id="9016e-151">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9016e-151">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="9016e-152">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9016e-152">Properties</span></span>

| <span data-ttu-id="9016e-153">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9016e-153">Property</span></span> | <span data-ttu-id="9016e-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="9016e-154">Type</span></span> | <span data-ttu-id="9016e-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="9016e-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9016e-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="9016e-156">extensionName</span></span>|<span data-ttu-id="9016e-157">String</span><span class="sxs-lookup"><span data-stu-id="9016e-157">String</span></span>|<span data-ttu-id="9016e-p106">Um identificador de texto exclusivo para uma extensão de dados de tipo aberto. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9016e-p106">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="9016e-160">id</span><span class="sxs-lookup"><span data-stu-id="9016e-160">id</span></span>|<span data-ttu-id="9016e-161">String</span><span class="sxs-lookup"><span data-stu-id="9016e-161">String</span></span>| <span data-ttu-id="9016e-p107">Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9016e-p107">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9016e-164">Relações</span><span class="sxs-lookup"><span data-stu-id="9016e-164">Relationships</span></span>

<span data-ttu-id="9016e-165">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9016e-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="9016e-166">Métodos</span><span class="sxs-lookup"><span data-stu-id="9016e-166">Methods</span></span>

| <span data-ttu-id="9016e-167">Método</span><span class="sxs-lookup"><span data-stu-id="9016e-167">Method</span></span> | <span data-ttu-id="9016e-168">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9016e-168">Return Type</span></span> | <span data-ttu-id="9016e-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="9016e-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="9016e-170">Post</span><span class="sxs-lookup"><span data-stu-id="9016e-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="9016e-171">[openTypeExtension](opentypeextension.md) (em uma instância de recurso existente) ou um novo [contato](../resources/contact.md), [evento](../resources/event.md)ou [mensagem](../resources/message.md) que contém um objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="9016e-171">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="9016e-172">Crie um objeto openTypeExtension em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="9016e-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="9016e-173">Get</span><span class="sxs-lookup"><span data-stu-id="9016e-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="9016e-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="9016e-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="9016e-175">Leia propriedades e relações do objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="9016e-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="9016e-176">Update</span><span class="sxs-lookup"><span data-stu-id="9016e-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="9016e-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="9016e-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="9016e-178">Atualize o objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="9016e-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="9016e-179">Excluir</span><span class="sxs-lookup"><span data-stu-id="9016e-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="9016e-180">None</span><span class="sxs-lookup"><span data-stu-id="9016e-180">None</span></span> |<span data-ttu-id="9016e-181">Exclua um objeto openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="9016e-181">Delete openTypeExtension object.</span></span> |

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
