---
title: Visão geral das propriedades estendidas do Outlook
description: 'Propriedades estendidas permitem o armazenamento de dados personalizados e especificamente servem como um mecanismo de fallback para os aplicativos acessarem '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 1b6364fd42b72e175a58bfcd28c0bdacc5e9629e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866830"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="fce11-103">Visão geral das propriedades estendidas do Outlook</span><span class="sxs-lookup"><span data-stu-id="fce11-103">Outlook extended properties overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fce11-p101">Propriedades estendidas permitem armazenar dados personalizados e servem especificamente como um mecanismo de fallback para os aplicativos acessarem dados personalizados de propriedades MAPI do Outlook quando essas propriedades _ainda não estão expostas nos metadados da API do Microsoft Graph_. Você pode usar a API REST de propriedades estendidas para armazenar ou obter esses dados personalizados nos seguintes recursos de usuário:</span><span class="sxs-lookup"><span data-stu-id="fce11-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="fce11-106">message</span><span class="sxs-lookup"><span data-stu-id="fce11-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="fce11-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="fce11-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="fce11-108">event</span><span class="sxs-lookup"><span data-stu-id="fce11-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="fce11-109">calendar</span><span class="sxs-lookup"><span data-stu-id="fce11-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="fce11-110">contact</span><span class="sxs-lookup"><span data-stu-id="fce11-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="fce11-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="fce11-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="fce11-112">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="fce11-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="fce11-113">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="fce11-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="fce11-114">Ou, nos seguintes recursos de grupo do Office 365:</span><span class="sxs-lookup"><span data-stu-id="fce11-114">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="fce11-115">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="fce11-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="fce11-116">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fce11-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="fce11-117">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="fce11-117">group [post](../resources/post.md)</span></span>

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="fce11-118">Usar propriedades estendidas ou extensões abertas?</span><span class="sxs-lookup"><span data-stu-id="fce11-118">Use extended properties or open extensions?</span></span>

<span data-ttu-id="fce11-p102">Nos cenários mais comuns, você deve ser capaz de usar extensões abertas (representadas por [openTypeExtension](../resources/opentypeextension.md), anteriormente conhecidas como extensões de dados do Office 365) para armazenar e acessar dados personalizados de instâncias de recursos na caixa de correio do usuário. Use propriedades estendidas somente se você precisar acessar dados personalizados para as propriedades MAPI do Outlook que ainda não estão expostas nos [metadados da API do Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api).</span><span class="sxs-lookup"><span data-stu-id="fce11-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="fce11-121">Tipos de propriedades estendidas</span><span class="sxs-lookup"><span data-stu-id="fce11-121">Types of extended properties</span></span>

<span data-ttu-id="fce11-122">Dependendo se você pretende armazenar um único valor ou vários valores (do mesmo tipo) em uma propriedade estendida, pode criar uma propriedade estendida como uma [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) ou uma [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="fce11-122">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="fce11-123">Cada um desses tipos identifica a propriedade por sua **id** e armazena dados em **value**.</span><span class="sxs-lookup"><span data-stu-id="fce11-123">Each of these types identifies the property by its **id** and stores data in **value**.</span></span>

<span data-ttu-id="fce11-124">Você pode usar **id** para obter uma instância de recurso específica em conjunto com essa propriedade estendida ou para filtrar em uma propriedade estendida de valor único para obter todas as instâncias que possuem essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="fce11-124">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span>

<span data-ttu-id="fce11-125">**Observação** Não é possível usar a API REST para obter todas as propriedades estendidas de uma instância específica em uma única chamada.</span><span class="sxs-lookup"><span data-stu-id="fce11-125">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>


### <a name="id-formats"></a><span data-ttu-id="fce11-126">formatos de id</span><span class="sxs-lookup"><span data-stu-id="fce11-126">id formats</span></span>

<span data-ttu-id="fce11-127">Você pode especificar o **id** de uma propriedade estendida em um dos três formatos:</span><span class="sxs-lookup"><span data-stu-id="fce11-127">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="fce11-128">Como uma propriedade nomeada, identificada pelo tipo de propriedade estendida, namespace e nome de uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="fce11-128">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="fce11-129">Como uma propriedade nomeada, identificada pelo tipo de propriedade estendida, namespace e um identificador numérico.</span><span class="sxs-lookup"><span data-stu-id="fce11-129">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="fce11-130">Em um formato de proptag, identificado pelo tipo de propriedade estendida e uma [marca de propriedade MAPI](/office/client-developer/outlook/mapi/mapi-property-tags).</span><span class="sxs-lookup"><span data-stu-id="fce11-130">In a proptag format, identified by the extended property type and a [MAPI property tag](/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="fce11-131">As próximas 2 tabelas descrevem esses formatos aplicados a propriedades estendidas única e com vários valores.</span><span class="sxs-lookup"><span data-stu-id="fce11-131">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="fce11-132">{_tipo_} representa o tipo de valor ou valores da propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="fce11-132">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="fce11-133">Os exemplos mostram a cadeia de caracteres, inteiro e matrizes desses tipos.</span><span class="sxs-lookup"><span data-stu-id="fce11-133">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="fce11-134">**Formatos de id válidos para propriedades estendidas de valor único**</span><span class="sxs-lookup"><span data-stu-id="fce11-134">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="fce11-135">**Formato**</span><span class="sxs-lookup"><span data-stu-id="fce11-135">**Format**</span></span>|<span data-ttu-id="fce11-136">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="fce11-136">**Example**</span></span>|<span data-ttu-id="fce11-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fce11-137">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="fce11-138">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="fce11-138">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="fce11-139">Identifica uma propriedade namespace (GUID) à qual ele pertence, e um nome de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="fce11-139">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="fce11-140">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="fce11-140">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="fce11-141">Identifica uma propriedade namespace (GUID) à qual ele pertence, e um identificador numérico.</span><span class="sxs-lookup"><span data-stu-id="fce11-141">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="fce11-142">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="fce11-142">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="fce11-143">Identifica uma propriedade predefinida por sua marca de propriedade.</span><span class="sxs-lookup"><span data-stu-id="fce11-143">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="fce11-144">**Formatos de id válidos para propriedades estendidas de vários valores**</span><span class="sxs-lookup"><span data-stu-id="fce11-144">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="fce11-145">**Formato**</span><span class="sxs-lookup"><span data-stu-id="fce11-145">**Format**</span></span>|<span data-ttu-id="fce11-146">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="fce11-146">**Example**</span></span>|<span data-ttu-id="fce11-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fce11-147">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="fce11-148">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="fce11-148">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="fce11-149">Identifica uma propriedade namespace (GUID) e um nome de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="fce11-149">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="fce11-150">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="fce11-150">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="fce11-151">Identifica uma propriedade namespace (GUID) e um identificador numérico.</span><span class="sxs-lookup"><span data-stu-id="fce11-151">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="fce11-152">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="fce11-152">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="fce11-153">Identifica uma propriedade predefinida por sua marca de propriedade.</span><span class="sxs-lookup"><span data-stu-id="fce11-153">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="fce11-154">Use qualquer um dos formatos de propriedade nomeada para definir uma propriedade estendida de valor único ou vários valores como uma propriedade personalizada.</span><span class="sxs-lookup"><span data-stu-id="fce11-154">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="fce11-155">Entre os dois formatos, o primeiro que leva o nome da cadeia de caracteres (**Nome**) é o formato preferencial para facilitar a referência.</span><span class="sxs-lookup"><span data-stu-id="fce11-155">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="fce11-156">Propriedades nomeadas tem seus [identificadores de propriedade](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) no intervalo 0x8000-0xfffe.</span><span class="sxs-lookup"><span data-stu-id="fce11-156">Named properties have their [property identifiers](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="fce11-157">Use o formato proptag para acessar propriedades predefinidas por MAPI ou por um cliente ou servidor e que já não tenha sido exibida no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fce11-157">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="fce11-158">Essas propriedades tem identificadores de propriedade no intervalo 0x0001-0x7fff.</span><span class="sxs-lookup"><span data-stu-id="fce11-158">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="fce11-159">Não tente definir uma propriedade personalizada usando o formato proptag.</span><span class="sxs-lookup"><span data-stu-id="fce11-159">Do not try to define a custom property using the proptag format.</span></span>

<span data-ttu-id="fce11-160">Você pode encontrar informações sobre o mapeamento de uma propriedade estendida para uma propriedade MAPI existente, como o identificador de propriedade e o GUID, na publicação da Microsoft Corporation \[MS-OXPROPS\], ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="fce11-160">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="fce11-161">**Observação** Depois de escolher um formato para a **id**, você deve acessar essa propriedade estendida apenas com esse formato.</span><span class="sxs-lookup"><span data-stu-id="fce11-161">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="fce11-162">Operações da API REST</span><span class="sxs-lookup"><span data-stu-id="fce11-162">REST API operations</span></span>

<span data-ttu-id="fce11-163">Operações de propriedades estendidas de valor único:</span><span class="sxs-lookup"><span data-stu-id="fce11-163">Single-value extended property operations:</span></span>

- [<span data-ttu-id="fce11-164">Criar uma propriedade estendida em uma instância de recurso nova ou existente</span><span class="sxs-lookup"><span data-stu-id="fce11-164">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="fce11-165">Obter uma instância de recurso, ou uma coleção delas, com uma propriedade estendida usando `$expand` ou `$filter`</span><span class="sxs-lookup"><span data-stu-id="fce11-165">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="fce11-166">Operações de propriedades estendidas de vários valores:</span><span class="sxs-lookup"><span data-stu-id="fce11-166">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="fce11-167">Criar uma propriedade estendida em uma instância de recurso nova ou existente</span><span class="sxs-lookup"><span data-stu-id="fce11-167">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- <span data-ttu-id="fce11-168">[Obter uma instância de recurso com uma propriedade estendida usando `$expand`](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="fce11-168">[Get a resource instance with an extended property using `$expand`](../api/multivaluelegacyextendedproperty-get.md)</span></span>

