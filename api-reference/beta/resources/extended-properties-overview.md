---
title: Visão geral das propriedades estendidas do Outlook
description: 'Propriedades estendidas permitem o armazenamento de dados personalizados e especificamente servem como um mecanismo de fallback para os aplicativos acessarem '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: d6e4cd91e8195530f6138bdd068907988b42c237
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499012"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="5eee7-103">Visão geral das propriedades estendidas do Outlook</span><span class="sxs-lookup"><span data-stu-id="5eee7-103">Outlook extended properties overview</span></span>

<span data-ttu-id="5eee7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5eee7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eee7-p101">Propriedades estendidas permitem armazenar dados personalizados e servem especificamente como um mecanismo de fallback para os aplicativos acessarem dados personalizados de propriedades MAPI do Outlook quando essas propriedades _ainda não estão expostas nos metadados da API do Microsoft Graph_. Você pode usar a API REST de propriedades estendidas para armazenar ou obter esses dados personalizados nos seguintes recursos de usuário:</span><span class="sxs-lookup"><span data-stu-id="5eee7-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="5eee7-107">message</span><span class="sxs-lookup"><span data-stu-id="5eee7-107">message</span></span>](../resources/message.md)
- [<span data-ttu-id="5eee7-108">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5eee7-108">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="5eee7-109">event</span><span class="sxs-lookup"><span data-stu-id="5eee7-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="5eee7-110">calendar</span><span class="sxs-lookup"><span data-stu-id="5eee7-110">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="5eee7-111">contact</span><span class="sxs-lookup"><span data-stu-id="5eee7-111">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="5eee7-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5eee7-112">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="5eee7-113">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="5eee7-113">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="5eee7-114">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="5eee7-114">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="5eee7-115">Ou, nos seguintes recursos de grupo do Office 365:</span><span class="sxs-lookup"><span data-stu-id="5eee7-115">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="5eee7-116">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="5eee7-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="5eee7-117">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="5eee7-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="5eee7-118">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="5eee7-118">group [post](../resources/post.md)</span></span>

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="5eee7-119">Usar propriedades estendidas ou extensões abertas?</span><span class="sxs-lookup"><span data-stu-id="5eee7-119">Use extended properties or open extensions?</span></span>

<span data-ttu-id="5eee7-p102">Nos cenários mais comuns, você deve ser capaz de usar extensões abertas (representadas por [openTypeExtension](../resources/opentypeextension.md), anteriormente conhecidas como extensões de dados do Office 365) para armazenar e acessar dados personalizados de instâncias de recursos na caixa de correio do usuário. Use propriedades estendidas somente se você precisar acessar dados personalizados para as propriedades MAPI do Outlook que ainda não estão expostas nos [metadados da API do Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api).</span><span class="sxs-lookup"><span data-stu-id="5eee7-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="5eee7-122">Tipos de propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="5eee7-122">Types of extended properties</span></span>

<span data-ttu-id="5eee7-123">Dependendo se você pretende armazenar um único valor ou vários valores (do mesmo tipo) em uma propriedade estendida, pode criar uma propriedade estendida como uma [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) ou uma [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="5eee7-123">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="5eee7-124">Cada um desses tipos identifica a propriedade por sua **id** e armazena dados em **value**.</span><span class="sxs-lookup"><span data-stu-id="5eee7-124">Each of these types identifies the property by its **id** and stores data in **value**.</span></span>

<span data-ttu-id="5eee7-125">Você pode usar **id** para obter uma instância de recurso específica em conjunto com essa propriedade estendida ou para filtrar em uma propriedade estendida de valor único para obter todas as instâncias que possuem essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="5eee7-125">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span>

<span data-ttu-id="5eee7-126">**Observação** Não é possível usar a API REST para obter todas as propriedades estendidas de uma instância específica em uma única chamada.</span><span class="sxs-lookup"><span data-stu-id="5eee7-126">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>


### <a name="id-formats"></a><span data-ttu-id="5eee7-127">formatos de id</span><span class="sxs-lookup"><span data-stu-id="5eee7-127">id formats</span></span>

<span data-ttu-id="5eee7-128">Você pode especificar o **id** de uma propriedade estendida em um dos três formatos:</span><span class="sxs-lookup"><span data-stu-id="5eee7-128">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="5eee7-129">Como uma propriedade nomeada, identificada pelo tipo de propriedade estendida, namespace e nome de uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="5eee7-129">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="5eee7-130">Como uma propriedade nomeada, identificada pelo tipo de propriedade estendida, namespace e um identificador numérico.</span><span class="sxs-lookup"><span data-stu-id="5eee7-130">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="5eee7-131">Em um formato de proptag, identificado pelo tipo de propriedade estendida e uma [marca de propriedade MAPI](/office/client-developer/outlook/mapi/mapi-property-tags).</span><span class="sxs-lookup"><span data-stu-id="5eee7-131">In a proptag format, identified by the extended property type and a [MAPI property tag](/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="5eee7-132">As próximas 2 tabelas descrevem esses formatos aplicados a propriedades estendidas única e com vários valores.</span><span class="sxs-lookup"><span data-stu-id="5eee7-132">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="5eee7-133">{_tipo_} representa o tipo de valor ou valores da propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="5eee7-133">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="5eee7-134">Os exemplos mostram a cadeia de caracteres, inteiro e matrizes desses tipos.</span><span class="sxs-lookup"><span data-stu-id="5eee7-134">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="5eee7-135">**Formatos de id válidos para propriedades estendidas de valor único**</span><span class="sxs-lookup"><span data-stu-id="5eee7-135">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="5eee7-136">**Formato**</span><span class="sxs-lookup"><span data-stu-id="5eee7-136">**Format**</span></span>|<span data-ttu-id="5eee7-137">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="5eee7-137">**Example**</span></span>|<span data-ttu-id="5eee7-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5eee7-138">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="5eee7-139">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="5eee7-139">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="5eee7-140">Identifica uma propriedade namespace (GUID) à qual ele pertence, e um nome de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="5eee7-140">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="5eee7-141">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="5eee7-141">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="5eee7-142">Identifica uma propriedade namespace (GUID) à qual ele pertence, e um identificador numérico.</span><span class="sxs-lookup"><span data-stu-id="5eee7-142">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="5eee7-143">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="5eee7-143">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="5eee7-144">Identifica uma propriedade predefinida por sua marca de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5eee7-144">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="5eee7-145">**Formatos de id válidos para propriedades estendidas de vários valores**</span><span class="sxs-lookup"><span data-stu-id="5eee7-145">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="5eee7-146">**Formato**</span><span class="sxs-lookup"><span data-stu-id="5eee7-146">**Format**</span></span>|<span data-ttu-id="5eee7-147">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="5eee7-147">**Example**</span></span>|<span data-ttu-id="5eee7-148">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5eee7-148">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="5eee7-149">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="5eee7-149">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="5eee7-150">Identifica uma propriedade namespace (GUID) e um nome de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="5eee7-150">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="5eee7-151">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="5eee7-151">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="5eee7-152">Identifica uma propriedade namespace (GUID) e um identificador numérico.</span><span class="sxs-lookup"><span data-stu-id="5eee7-152">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="5eee7-153">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="5eee7-153">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="5eee7-154">Identifica uma propriedade predefinida por sua marca de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5eee7-154">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="5eee7-155">Use qualquer um dos formatos de propriedade nomeada para definir uma propriedade estendida de valor único ou vários valores como uma propriedade personalizada.</span><span class="sxs-lookup"><span data-stu-id="5eee7-155">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="5eee7-156">Entre os dois formatos, o primeiro que leva o nome da cadeia de caracteres (**Nome**) é o formato preferencial para facilitar a referência.</span><span class="sxs-lookup"><span data-stu-id="5eee7-156">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="5eee7-157">Propriedades nomeadas tem seus [identificadores de propriedade](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) no intervalo 0x8000-0xfffe.</span><span class="sxs-lookup"><span data-stu-id="5eee7-157">Named properties have their [property identifiers](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="5eee7-158">Use o formato proptag para acessar propriedades predefinidas por MAPI ou por um cliente ou servidor e que já não tenha sido exibida no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5eee7-158">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="5eee7-159">Essas propriedades tem identificadores de propriedade no intervalo 0x0001-0x7fff.</span><span class="sxs-lookup"><span data-stu-id="5eee7-159">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="5eee7-160">Não tente definir uma propriedade personalizada usando o formato proptag.</span><span class="sxs-lookup"><span data-stu-id="5eee7-160">Do not try to define a custom property using the proptag format.</span></span>

<span data-ttu-id="5eee7-161">Você pode encontrar informações sobre o mapeamento de uma propriedade estendida para uma propriedade MAPI existente, como o identificador de propriedade e o GUID, na publicação da Microsoft Corporation \[MS-OXPROPS\], ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="5eee7-161">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="5eee7-162">**Observação** Depois de escolher um formato para a **id**, você deve acessar essa propriedade estendida apenas com esse formato.</span><span class="sxs-lookup"><span data-stu-id="5eee7-162">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="5eee7-163">Operações da API REST</span><span class="sxs-lookup"><span data-stu-id="5eee7-163">REST API operations</span></span>

<span data-ttu-id="5eee7-164">Operações de propriedades estendidas de valor único:</span><span class="sxs-lookup"><span data-stu-id="5eee7-164">Single-value extended property operations:</span></span>

- [<span data-ttu-id="5eee7-165">Criar uma propriedade estendida em uma instância de recurso nova ou existente</span><span class="sxs-lookup"><span data-stu-id="5eee7-165">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="5eee7-166">Obter uma instância de recurso, ou uma coleção delas, com uma propriedade estendida usando `$expand` ou `$filter`</span><span class="sxs-lookup"><span data-stu-id="5eee7-166">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="5eee7-167">Operações de propriedades estendidas de vários valores:</span><span class="sxs-lookup"><span data-stu-id="5eee7-167">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="5eee7-168">Criar uma propriedade estendida em uma instância de recurso nova ou existente</span><span class="sxs-lookup"><span data-stu-id="5eee7-168">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- <span data-ttu-id="5eee7-169">[Obter uma instância de recurso com uma propriedade estendida usando `$expand`](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="5eee7-169">[Get a resource instance with an extended property using `$expand`](../api/multivaluelegacyextendedproperty-get.md)</span></span>

