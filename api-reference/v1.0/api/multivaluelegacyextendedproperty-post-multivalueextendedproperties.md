---
title: Criar propriedade estendida de vários valores
description: 'Crie uma ou mais propriedades estendidas de vários valores em uma instância nova ou existente de um recurso. '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d4e0d00fe59f74b0b53d116c5b2a34f73b94edcd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130540"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="34c1d-103">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="34c1d-103">Create multi-value extended property</span></span>

<span data-ttu-id="34c1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34c1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34c1d-105">Crie uma ou mais propriedades estendidas de vários valores em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="34c1d-105">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="34c1d-106">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="34c1d-106">The following user resources are supported:</span></span>

- [<span data-ttu-id="34c1d-107">calendar</span><span class="sxs-lookup"><span data-stu-id="34c1d-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="34c1d-108">contact</span><span class="sxs-lookup"><span data-stu-id="34c1d-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="34c1d-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="34c1d-109">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="34c1d-110">event</span><span class="sxs-lookup"><span data-stu-id="34c1d-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="34c1d-111">mailFolder</span><span class="sxs-lookup"><span data-stu-id="34c1d-111">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="34c1d-112">message</span><span class="sxs-lookup"><span data-stu-id="34c1d-112">message</span></span>](../resources/message.md)

<span data-ttu-id="34c1d-113">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="34c1d-113">As well as the following group resources:</span></span>

- <span data-ttu-id="34c1d-114">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="34c1d-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="34c1d-115">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="34c1d-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="34c1d-116">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="34c1d-116">group [post](../resources/post.md)</span></span>

<span data-ttu-id="34c1d-117">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="34c1d-117">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="34c1d-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="34c1d-118">Permissions</span></span>
<span data-ttu-id="34c1d-119">Dependendo do recurso no qual você está criando a propriedade estendida e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="34c1d-119">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="34c1d-120">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34c1d-120">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34c1d-121">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="34c1d-121">Supported resource</span></span> | <span data-ttu-id="34c1d-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34c1d-122">Delegated (work or school account)</span></span> | <span data-ttu-id="34c1d-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34c1d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34c1d-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34c1d-124">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="34c1d-125">calendar</span><span class="sxs-lookup"><span data-stu-id="34c1d-125">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="34c1d-126">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-126">Calendars.ReadWrite</span></span> | <span data-ttu-id="34c1d-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="34c1d-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-128">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="34c1d-129">contato</span><span class="sxs-lookup"><span data-stu-id="34c1d-129">contact</span></span>](../resources/contact.md) | <span data-ttu-id="34c1d-130">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-130">Contacts.ReadWrite</span></span> | <span data-ttu-id="34c1d-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="34c1d-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-132">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="34c1d-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="34c1d-133">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="34c1d-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="34c1d-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="34c1d-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-136">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="34c1d-137">evento</span><span class="sxs-lookup"><span data-stu-id="34c1d-137">event</span></span>](../resources/event.md) | <span data-ttu-id="34c1d-138">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-138">Calendars.ReadWrite</span></span> | <span data-ttu-id="34c1d-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-139">Calendars.ReadWrite</span></span> |  <span data-ttu-id="34c1d-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-140">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="34c1d-141">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="34c1d-141">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="34c1d-142">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34c1d-142">Group.ReadWrite.All</span></span> | <span data-ttu-id="34c1d-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="34c1d-143">Not supported</span></span> | <span data-ttu-id="34c1d-144">Incompatível</span><span class="sxs-lookup"><span data-stu-id="34c1d-144">Not supported</span></span> |
| <span data-ttu-id="34c1d-145">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="34c1d-145">group [event](../resources/event.md)</span></span> | <span data-ttu-id="34c1d-146">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34c1d-146">Group.ReadWrite.All</span></span> | <span data-ttu-id="34c1d-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="34c1d-147">Not supported</span></span> | <span data-ttu-id="34c1d-148">Incompatível</span><span class="sxs-lookup"><span data-stu-id="34c1d-148">Not supported</span></span> |
| <span data-ttu-id="34c1d-149">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="34c1d-149">group [post](../resources/post.md)</span></span> | <span data-ttu-id="34c1d-150">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34c1d-150">Group.ReadWrite.All</span></span> | <span data-ttu-id="34c1d-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="34c1d-151">Not supported</span></span> | <span data-ttu-id="34c1d-152">Incompatível</span><span class="sxs-lookup"><span data-stu-id="34c1d-152">Not supported</span></span> |
| [<span data-ttu-id="34c1d-153">mailFolder</span><span class="sxs-lookup"><span data-stu-id="34c1d-153">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="34c1d-154">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-154">Mail.ReadWrite</span></span> | <span data-ttu-id="34c1d-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-155">Mail.ReadWrite</span></span> | <span data-ttu-id="34c1d-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-156">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="34c1d-157">mensagem</span><span class="sxs-lookup"><span data-stu-id="34c1d-157">message</span></span>](../resources/message.md) | <span data-ttu-id="34c1d-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-158">Mail.ReadWrite</span></span> | <span data-ttu-id="34c1d-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-159">Mail.ReadWrite</span></span> | <span data-ttu-id="34c1d-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c1d-160">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="34c1d-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34c1d-161">HTTP request</span></span>
<span data-ttu-id="34c1d-162">Você pode criar propriedades estendidas em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="34c1d-162">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="34c1d-p102">Para criar uma ou mais propriedades estendidas em uma _nova_ instância de recurso, use a mesma solicitação REST válida para a criação da instância e inclua as propriedades da nova instância de recurso _e a propriedade estendida_ no corpo da solicitação. Observe que alguns recursos dão suporte à criação de mais de uma maneira. Para saber mais sobre como criar essas instâncias de recurso, confira os tópicos correspondentes para a criação de [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md) e [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="34c1d-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span>

<span data-ttu-id="34c1d-166">Veja a seguir a sintaxe das solicitações.</span><span class="sxs-lookup"><span data-stu-id="34c1d-166">The following is the syntax of the requests.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="34c1d-167">Para criar uma ou mais propriedades estendidas em uma instância de recurso existente, especifique essa instância na solicitação e inclua a propriedade estendida no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34c1d-167">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="34c1d-168">**Observação** Não é possível criar uma propriedade estendida em uma postagem de grupo existente.</span><span class="sxs-lookup"><span data-stu-id="34c1d-168">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="34c1d-169">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34c1d-169">Request headers</span></span>
| <span data-ttu-id="34c1d-170">Nome</span><span class="sxs-lookup"><span data-stu-id="34c1d-170">Name</span></span>       | <span data-ttu-id="34c1d-171">Valor</span><span class="sxs-lookup"><span data-stu-id="34c1d-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="34c1d-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="34c1d-172">Authorization</span></span> | <span data-ttu-id="34c1d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34c1d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34c1d-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34c1d-175">Content-Type</span></span> | <span data-ttu-id="34c1d-176">application/json</span><span class="sxs-lookup"><span data-stu-id="34c1d-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="34c1d-177">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34c1d-177">Request body</span></span>

<span data-ttu-id="34c1d-178">Forneça um corpo JSON de cada objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) na propriedade da coleção **multiValueExtendedProperties** da instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="34c1d-178">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="34c1d-179">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34c1d-179">Property</span></span>|<span data-ttu-id="34c1d-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="34c1d-180">Type</span></span>|<span data-ttu-id="34c1d-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="34c1d-181">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="34c1d-182">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="34c1d-182">multiValueExtendedProperties</span></span>|<span data-ttu-id="34c1d-183">Coleção [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="34c1d-183">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="34c1d-184">Uma matriz de uma ou mais propriedades estendidas de vários valores.</span><span class="sxs-lookup"><span data-stu-id="34c1d-184">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="34c1d-185">id</span><span class="sxs-lookup"><span data-stu-id="34c1d-185">id</span></span>|<span data-ttu-id="34c1d-186">String</span><span class="sxs-lookup"><span data-stu-id="34c1d-186">String</span></span>|<span data-ttu-id="34c1d-p104">Para cada propriedade na coleção **multiValueExtendedProperties**, especifique isso para identificar a propriedade. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34c1d-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="34c1d-191">valor</span><span class="sxs-lookup"><span data-stu-id="34c1d-191">value</span></span>|<span data-ttu-id="34c1d-192">string</span><span class="sxs-lookup"><span data-stu-id="34c1d-192">string</span></span>|<span data-ttu-id="34c1d-p105">Para cada propriedade na coleção **multiValueExtendedProperties**, especifique o valor da propriedade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34c1d-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="34c1d-195">Ao criar uma propriedade  estendida em uma nova instância de recurso, além da nova coleção **multiValueExtendedProperties,** forneça uma representação JSON dessa instância de recurso também (ou seja, uma mensagem [,](../resources/message.md) [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md)etc.).</span><span class="sxs-lookup"><span data-stu-id="34c1d-195">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance as well (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.).</span></span>


## <a name="response"></a><span data-ttu-id="34c1d-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="34c1d-196">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="34c1d-197">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="34c1d-197">Response code</span></span>
<span data-ttu-id="34c1d-198">Uma operação bem-sucedida na criação de uma propriedade estendida em uma nova instância de recurso retorna `201 Created`, exceto em uma nova postagem de grupo. Dependendo do método usado, a operação pode retornar `200 OK` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="34c1d-198">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="34c1d-199">Em uma instância de recurso existente, uma operação de criação bem-sucedida retorna `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="34c1d-199">In an existing resource instance, a successful create operation returns `200 OK`.</span></span>


#### <a name="response-body"></a><span data-ttu-id="34c1d-200">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="34c1d-200">Response body</span></span>

<span data-ttu-id="34c1d-p106">Ao criar uma propriedade estendida em um recurso com suporte que não seja [group post](../resources/post.md), a resposta inclui apenas a instância nova ou existente, mas não a nova propriedade estendida. Para ver a propriedade estendida recém-criada, [obtenha a instância expandida com a propriedade estendida](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="34c1d-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="34c1d-p107">Ao criar uma propriedade estendida em uma _nova_ postagem de grupo, a resposta inclui um código de resposta, mas não a nova postagem nem a propriedade estendida. Não é possível criar uma propriedade estendida em uma postagem de grupo existente.</span><span class="sxs-lookup"><span data-stu-id="34c1d-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="34c1d-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34c1d-205">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="34c1d-206">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="34c1d-206">Request 1</span></span>

<span data-ttu-id="34c1d-p108">O primeiro exemplo cria uma propriedade estendida de vários valores em um novo evento, tudo na mesma operação POST. Além das propriedades que você normalmente incluiria para um novo evento, o corpo da solicitação inclui a coleção **multiValueExtendedProperties**, que contém uma propriedade estendida. O corpo da solicitação inclui o seguinte para essa propriedade estendida de vários valores:</span><span class="sxs-lookup"><span data-stu-id="34c1d-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="34c1d-210">**id**, que especifica a propriedade como uma matriz de cadeias de caracteres com o GUID especificado e o nome `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="34c1d-210">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span>
- <span data-ttu-id="34c1d-211">**value**, que especifica `Recreation` como uma matriz de 3 valores de cadeia de caracteres, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="34c1d-211">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="34c1d-212">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="34c1d-212">Response 1</span></span>

<span data-ttu-id="34c1d-p109">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 201 Created` e inclui o novo evento em seu corpo, semelhante à resposta da [criação de apenas um evento](../api/user-post-events.md). A resposta não inclui propriedades estendidas recém-criadas.</span><span class="sxs-lookup"><span data-stu-id="34c1d-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="34c1d-215">Para ver a propriedade estendida recém-criada, [obtenha o evento expandido com a propriedade estendida](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="34c1d-215">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="34c1d-216">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="34c1d-216">Request 2</span></span>

<span data-ttu-id="34c1d-p110">O segundo exemplo cria uma propriedade estendida de vários valores para a mensagem especificada. Essa propriedade estendida é o único elemento na coleção **multiValueExtendedProperties**. O corpo da solicitação inclui o seguinte para essa propriedade estendida:</span><span class="sxs-lookup"><span data-stu-id="34c1d-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="34c1d-220">**id** especifica a propriedade como uma matriz de cadeias de caracteres com o GUID especificado e o nome `Palette`.</span><span class="sxs-lookup"><span data-stu-id="34c1d-220">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="34c1d-221">**value** especifica `Palette` como uma matriz de 3 valores de cadeia de caracteres, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="34c1d-221">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="34c1d-222">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="34c1d-222">Response 2</span></span>

<span data-ttu-id="34c1d-p111">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK` e inclui a mensagem especificada em seu corpo, semelhante à resposta da [atualização de uma mensagem](../api/message-update.md). A resposta não inclui a propriedade estendida recém-criada.</span><span class="sxs-lookup"><span data-stu-id="34c1d-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="34c1d-225">Para ver a propriedade estendida recém-criada, [obtenha a mensagem expandida com a propriedade estendida](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="34c1d-225">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->





