---
title: Criar extensão aberta
description: Crie uma extensão aberta (objeto openTypeExtension) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 8a95fe4318409a613a05cd4d581aa366d0b138d0
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092432"
---
# <a name="create-open-extension"></a><span data-ttu-id="19a70-103">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="19a70-103">Create open extension</span></span>

<span data-ttu-id="19a70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19a70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19a70-105">Crie uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="19a70-105">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="19a70-106">A tabela na seção [Permissões](#permissions) lista os recursos que oferecem suporte a extensões abertas.</span><span class="sxs-lookup"><span data-stu-id="19a70-106">The table in the [Permissions](#permissions) section lists the resources that support open extensions.</span></span>

> <span data-ttu-id="19a70-107">**Observação:** Se você estiver criando extensões abertas em recursos do Outlook, confira **considerações específicas do Outlook** no [tipo de recurso openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="19a70-107">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="19a70-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="19a70-108">Permissions</span></span>

<span data-ttu-id="19a70-109">Dependendo do recurso para o qual você está criando a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="19a70-109">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="19a70-110">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19a70-110">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19a70-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="19a70-111">Supported resource</span></span> | <span data-ttu-id="19a70-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19a70-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19a70-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19a70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a70-114">Application</span><span class="sxs-lookup"><span data-stu-id="19a70-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="19a70-115">device</span><span class="sxs-lookup"><span data-stu-id="19a70-115">device</span></span>](../resources/device.md) | <span data-ttu-id="19a70-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19a70-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="19a70-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="19a70-117">Not supported</span></span> | <span data-ttu-id="19a70-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="19a70-119">evento</span><span class="sxs-lookup"><span data-stu-id="19a70-119">event</span></span>](../resources/event.md) | <span data-ttu-id="19a70-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="19a70-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="19a70-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="19a70-123">grupo</span><span class="sxs-lookup"><span data-stu-id="19a70-123">group</span></span>](../resources/group.md) | <span data-ttu-id="19a70-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="19a70-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="19a70-125">Not supported</span></span> | <span data-ttu-id="19a70-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="19a70-127">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="19a70-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="19a70-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="19a70-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="19a70-129">Not supported</span></span> | <span data-ttu-id="19a70-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="19a70-130">Not supported</span></span> |
| [<span data-ttu-id="19a70-131">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="19a70-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="19a70-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="19a70-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="19a70-133">Not supported</span></span> | <span data-ttu-id="19a70-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="19a70-135">mensagem</span><span class="sxs-lookup"><span data-stu-id="19a70-135">message</span></span>](../resources/message.md) | <span data-ttu-id="19a70-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-136">Mail.ReadWrite</span></span> | <span data-ttu-id="19a70-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-137">Mail.ReadWrite</span></span> | <span data-ttu-id="19a70-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="19a70-139">organization</span><span class="sxs-lookup"><span data-stu-id="19a70-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="19a70-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-140">Organization.ReadWrite.All</span></span> | <span data-ttu-id="19a70-141">Incompatível</span><span class="sxs-lookup"><span data-stu-id="19a70-141">Not supported</span></span> | <span data-ttu-id="19a70-142">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-142">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="19a70-143">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="19a70-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="19a70-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="19a70-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="19a70-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="19a70-147">user</span><span class="sxs-lookup"><span data-stu-id="19a70-147">user</span></span>](../resources/user.md) | <span data-ttu-id="19a70-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-148">User.ReadWrite</span></span> | <span data-ttu-id="19a70-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-149">User.ReadWrite</span></span> | <span data-ttu-id="19a70-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-150">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="19a70-151">tarefa</span><span class="sxs-lookup"><span data-stu-id="19a70-151">task</span></span>](../resources/todotask.md) | <span data-ttu-id="19a70-152">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-152">Tasks.ReadWrite</span></span> | <span data-ttu-id="19a70-153">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-153">Tasks.ReadWrite</span></span> | <span data-ttu-id="19a70-154">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-154">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="19a70-155">tasklist</span><span class="sxs-lookup"><span data-stu-id="19a70-155">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="19a70-156">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-156">Tasks.ReadWrite</span></span> | <span data-ttu-id="19a70-157">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a70-157">Tasks.ReadWrite</span></span> | <span data-ttu-id="19a70-158">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a70-158">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a70-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19a70-159">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="19a70-160">Crie uma extensão em uma nova instância de recurso</span><span class="sxs-lookup"><span data-stu-id="19a70-160">Create an extension in a new resource instance</span></span>

<span data-ttu-id="19a70-161">Use a mesma solicitação REST usada para criar a instância.</span><span class="sxs-lookup"><span data-stu-id="19a70-161">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
POST /users/{id|userPrincipalName}/todo/lists/{id}/tasks
POST /users/{id|userPrincipalName}/todo/lists
```

><span data-ttu-id="19a70-162">**Observação:** Esta sintaxe acima mostra algumas maneiras comuns de criar as instâncias de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="19a70-162">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="19a70-163">Todas as outras sintaxes POST que permitem criar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="19a70-163">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="19a70-164">Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a70-164">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="19a70-165">Crie uma extensão em uma instância de recurso existente</span><span class="sxs-lookup"><span data-stu-id="19a70-165">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="19a70-166">Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.</span><span class="sxs-lookup"><span data-stu-id="19a70-166">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
POST /users/{id|userPrincipalName}/todo/lists/{id}/tasks/{id}/extensions
POST /users/{id|userPrincipalName}/todo/lists/{id}/extensions
```

><span data-ttu-id="19a70-167">**Observação:** Esta sintaxe mostra algumas maneiras comuns de identificar uma instância do recurso, para criar uma extensão nele.</span><span class="sxs-lookup"><span data-stu-id="19a70-167">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="19a70-168">Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="19a70-168">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="19a70-169">Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a70-169">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="19a70-170">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="19a70-170">Path parameters</span></span>
|<span data-ttu-id="19a70-171">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="19a70-171">Parameter</span></span>|<span data-ttu-id="19a70-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="19a70-172">Type</span></span>|<span data-ttu-id="19a70-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="19a70-173">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="19a70-174">id</span><span class="sxs-lookup"><span data-stu-id="19a70-174">id</span></span>|<span data-ttu-id="19a70-175">string</span><span class="sxs-lookup"><span data-stu-id="19a70-175">string</span></span>|<span data-ttu-id="19a70-p104">Um identificador exclusivo para um objeto na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19a70-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="19a70-178">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19a70-178">Request headers</span></span>

| <span data-ttu-id="19a70-179">Nome</span><span class="sxs-lookup"><span data-stu-id="19a70-179">Name</span></span>       | <span data-ttu-id="19a70-180">Valor</span><span class="sxs-lookup"><span data-stu-id="19a70-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="19a70-181">Autorização</span><span class="sxs-lookup"><span data-stu-id="19a70-181">Authorization</span></span> | <span data-ttu-id="19a70-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19a70-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19a70-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19a70-184">Content-Type</span></span> | <span data-ttu-id="19a70-185">application/json</span><span class="sxs-lookup"><span data-stu-id="19a70-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a70-186">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19a70-186">Request body</span></span>

<span data-ttu-id="19a70-p106">Forneça um corpo JSON de uma [openTypeExtension](../resources/opentypeextension.md), com os seguintes pares de nome/valor obrigatórios e dados personalizados adicionais. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="19a70-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="19a70-189">Name</span><span class="sxs-lookup"><span data-stu-id="19a70-189">Name</span></span>       | <span data-ttu-id="19a70-190">Valor</span><span class="sxs-lookup"><span data-stu-id="19a70-190">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="19a70-191">@odata.type</span><span class="sxs-lookup"><span data-stu-id="19a70-191">@odata.type</span></span> | <span data-ttu-id="19a70-192">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="19a70-192">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="19a70-193">extensionName</span><span class="sxs-lookup"><span data-stu-id="19a70-193">extensionName</span></span> | <span data-ttu-id="19a70-194">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="19a70-194">%unique_string%</span></span> |

<span data-ttu-id="19a70-195">Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.</span><span class="sxs-lookup"><span data-stu-id="19a70-195">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="19a70-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a70-196">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="19a70-197">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="19a70-197">Response code</span></span>

<span data-ttu-id="19a70-198">Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="19a70-198">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="19a70-199">Quando você cria uma extensão usando a mesma operação usada para criar uma instância de recurso, a operação retorna o mesmo código de resposta retornado quando você usa a operação para criar a instância do recurso sem a extensão.</span><span class="sxs-lookup"><span data-stu-id="19a70-199">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="19a70-200">Consulte os tópicos correspondentes para criar a instância conforme listado [cima](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="19a70-200">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="19a70-201">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="19a70-201">Response body</span></span>

| <span data-ttu-id="19a70-202">Cenário</span><span class="sxs-lookup"><span data-stu-id="19a70-202">Scenario</span></span>       | <span data-ttu-id="19a70-203">Recurso</span><span class="sxs-lookup"><span data-stu-id="19a70-203">Resource</span></span>  | <span data-ttu-id="19a70-204">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="19a70-204">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="19a70-205">Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso</span><span class="sxs-lookup"><span data-stu-id="19a70-205">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="19a70-206">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="19a70-206">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="19a70-207">Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="19a70-207">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="19a70-208">Criando uma extensão ao criar implicitamente uma instância de recursos</span><span class="sxs-lookup"><span data-stu-id="19a70-208">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="19a70-209">postagem</span><span class="sxs-lookup"><span data-stu-id="19a70-209">post</span></span>](../resources/post.md) | <span data-ttu-id="19a70-210">A resposta inclui somente um código de resposta, mas não um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19a70-210">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="19a70-211">Criar uma extensão em uma instância de recurso _existente_</span><span class="sxs-lookup"><span data-stu-id="19a70-211">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="19a70-212">Todos os recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="19a70-212">All supported resources</span></span> | <span data-ttu-id="19a70-213">Inclui o objeto **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="19a70-213">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="19a70-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19a70-214">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="19a70-215">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="19a70-215">Request 1</span></span>

<span data-ttu-id="19a70-p108">O primeiro exemplo cria uma mensagem e uma extensão na mesma chamada. O corpo da solicitação inclui o seguinte:</span><span class="sxs-lookup"><span data-stu-id="19a70-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="19a70-218">As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="19a70-218">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="19a70-219">E para a extensão:</span><span class="sxs-lookup"><span data-stu-id="19a70-219">And for the extension:</span></span>

  - <span data-ttu-id="19a70-220">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="19a70-220">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="19a70-221">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="19a70-221">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="19a70-222">Dados adicionais a serem armazenados como três propriedades personalizadas no conteúdo JSON: `companyName`, `expirationDate` e `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="19a70-222">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="19a70-223">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="19a70-223">Response 1</span></span>

<span data-ttu-id="19a70-p109">Veja a seguir a resposta para o primeiro exemplo. O corpo da resposta inclui propriedades da nova mensagem e o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="19a70-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="19a70-226">A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="19a70-226">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="19a70-227">A propriedade padrão **extensionName** especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a70-227">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="19a70-228">Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="19a70-228">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="19a70-p110">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19a70-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
      "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="19a70-231">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="19a70-231">Request 2</span></span>

<span data-ttu-id="19a70-p111">O segundo exemplo cria uma extensão na mensagem especificada. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="19a70-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="19a70-234">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="19a70-234">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="19a70-235">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="19a70-235">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="19a70-236">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="19a70-236">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="19a70-237">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="19a70-237">Response 2</span></span>

<span data-ttu-id="19a70-p112">Veja a seguir a resposta para o segundo exemplo. O corpo da solicitação inclui o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="19a70-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="19a70-240">A propriedade padrão **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="19a70-240">The default property **extensionName**.</span></span>
- <span data-ttu-id="19a70-241">A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="19a70-241">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="19a70-242">Os dados personalizados a serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="19a70-242">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="19a70-243">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="19a70-243">Request 3</span></span>

<span data-ttu-id="19a70-p113">O terceiro exemplo cria uma extensão no evento de grupo especificado. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="19a70-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="19a70-246">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="19a70-246">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="19a70-247">O nome da extensão "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="19a70-247">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="19a70-248">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="19a70-248">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="19a70-249">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="19a70-249">Response 3</span></span>

<span data-ttu-id="19a70-250">Veja a seguir a resposta da terceira solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="19a70-250">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="19a70-251">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="19a70-251">Request 4</span></span>

<span data-ttu-id="19a70-p114">O quarto exemplo cria uma extensão em uma nova postagem de grupo, usando a mesma chamada de ação **reply** para uma postagem de grupo existente. A ação **reply** cria uma nova postagem e uma nova extensão inserida nessa postagem. O corpo da solicitação inclui uma propriedade **post** que, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="19a70-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="19a70-255">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="19a70-255">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="19a70-256">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="19a70-256">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="19a70-257">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="19a70-257">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```

### <a name="response-4"></a><span data-ttu-id="19a70-258">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="19a70-258">Response 4</span></span>

<span data-ttu-id="19a70-p115">Veja a seguir a resposta do quarto exemplo. Criar uma extensão com êxito em uma nova postagem de grupo resulta apenas no código de resposta HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="19a70-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a><span data-ttu-id="19a70-261">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="19a70-261">Request 5</span></span>

<span data-ttu-id="19a70-p116">O quinto exemplo cria uma extensão em uma nova postagem de grupo usando a mesma operação POST para criar uma conversa. A operação POST cria uma nova conversa, thread ou postagem e uma nova extensão inserida na postagem. O corpo da solicitação inclui as propriedades **Topic** e **Threads** e o objeto filho **post** para a nova conversa. O objeto **post**, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a extensão:</span><span class="sxs-lookup"><span data-stu-id="19a70-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="19a70-266">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="19a70-266">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="19a70-267">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="19a70-267">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="19a70-268">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="19a70-268">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "microsoft.graph.openTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="response-5"></a><span data-ttu-id="19a70-269">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="19a70-269">Response 5</span></span>

<span data-ttu-id="19a70-p117">Veja a seguir a resposta do quinto exemplo, que contém a nova conversa e uma ID de thread. Esse novo thread contém uma postagem criada automaticamente que, por sua vez, contém a nova extensão.</span><span class="sxs-lookup"><span data-stu-id="19a70-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="19a70-p118">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19a70-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="19a70-p119">Para obter a nova extensão, primeiro [obtenha todas as postagens](../api/conversationthread-list-posts.md) desse thread. Inicialmente, deve haver somente uma. Em seguida, aplique a ID da postagem e o nome da extensão `Com.Contoso.Benefits` para [obter a extensão](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="19a70-p119">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

