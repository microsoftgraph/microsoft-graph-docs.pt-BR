---
title: Criar extensão aberta
description: Crie uma extensão aberta (objeto openTypeExtension) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: f91a549e13b956d9c0d1fa4d8ca8765e7b7bd89a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052219"
---
# <a name="create-open-extension"></a><span data-ttu-id="170d9-103">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="170d9-103">Create open extension</span></span>

<span data-ttu-id="170d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="170d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="170d9-105">Crie uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="170d9-105">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="170d9-106">A tabela na seção [Permissões](#permissions) lista os recursos que oferecem suporte a extensões abertas.</span><span class="sxs-lookup"><span data-stu-id="170d9-106">The table in the [Permissions](#permissions) section lists the resources that support open extensions.</span></span>

> <span data-ttu-id="170d9-107">**Observação:** Se você estiver criando extensões abertas em recursos do Outlook, confira **considerações específicas do Outlook** no [tipo de recurso openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="170d9-107">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="170d9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="170d9-108">Permissions</span></span>

<span data-ttu-id="170d9-109">Dependendo do recurso para o qual você está criando a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="170d9-109">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="170d9-110">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="170d9-110">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="170d9-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="170d9-111">Supported resource</span></span> | <span data-ttu-id="170d9-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="170d9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="170d9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="170d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="170d9-114">Application</span><span class="sxs-lookup"><span data-stu-id="170d9-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="170d9-115">device</span><span class="sxs-lookup"><span data-stu-id="170d9-115">device</span></span>](../resources/device.md) | <span data-ttu-id="170d9-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="170d9-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="170d9-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="170d9-117">Not supported</span></span> | <span data-ttu-id="170d9-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="170d9-119">evento</span><span class="sxs-lookup"><span data-stu-id="170d9-119">event</span></span>](../resources/event.md) | <span data-ttu-id="170d9-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="170d9-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="170d9-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="170d9-123">grupo</span><span class="sxs-lookup"><span data-stu-id="170d9-123">group</span></span>](../resources/group.md) | <span data-ttu-id="170d9-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="170d9-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="170d9-125">Not supported</span></span> | <span data-ttu-id="170d9-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="170d9-127">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="170d9-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="170d9-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="170d9-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="170d9-129">Not supported</span></span> | <span data-ttu-id="170d9-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="170d9-130">Not supported</span></span> |
| [<span data-ttu-id="170d9-131">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="170d9-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="170d9-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="170d9-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="170d9-133">Not supported</span></span> | <span data-ttu-id="170d9-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="170d9-135">mensagem</span><span class="sxs-lookup"><span data-stu-id="170d9-135">message</span></span>](../resources/message.md) | <span data-ttu-id="170d9-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-136">Mail.ReadWrite</span></span> | <span data-ttu-id="170d9-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-137">Mail.ReadWrite</span></span> | <span data-ttu-id="170d9-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="170d9-139">organization</span><span class="sxs-lookup"><span data-stu-id="170d9-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="170d9-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-140">Organization.ReadWrite.All</span></span> | <span data-ttu-id="170d9-141">Incompatível</span><span class="sxs-lookup"><span data-stu-id="170d9-141">Not supported</span></span> | <span data-ttu-id="170d9-142">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-142">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="170d9-143">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="170d9-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="170d9-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="170d9-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="170d9-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="170d9-147">user</span><span class="sxs-lookup"><span data-stu-id="170d9-147">user</span></span>](../resources/user.md) | <span data-ttu-id="170d9-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-148">User.ReadWrite</span></span> | <span data-ttu-id="170d9-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-149">User.ReadWrite</span></span> | <span data-ttu-id="170d9-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-150">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="170d9-151">tarefa</span><span class="sxs-lookup"><span data-stu-id="170d9-151">task</span></span>](../resources/todotask.md) | <span data-ttu-id="170d9-152">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-152">Tasks.ReadWrite</span></span> | <span data-ttu-id="170d9-153">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-153">Tasks.ReadWrite</span></span> | <span data-ttu-id="170d9-154">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-154">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="170d9-155">tasklist</span><span class="sxs-lookup"><span data-stu-id="170d9-155">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="170d9-156">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-156">Tasks.ReadWrite</span></span> | <span data-ttu-id="170d9-157">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170d9-157">Tasks.ReadWrite</span></span> | <span data-ttu-id="170d9-158">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170d9-158">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="170d9-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="170d9-159">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="170d9-160">Crie uma extensão em uma nova instância de recurso</span><span class="sxs-lookup"><span data-stu-id="170d9-160">Create an extension in a new resource instance</span></span>

<span data-ttu-id="170d9-161">Use a mesma solicitação REST usada para criar a instância.</span><span class="sxs-lookup"><span data-stu-id="170d9-161">Use the same REST request that you use to create the instance.</span></span>

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

><span data-ttu-id="170d9-162">**Observação:** Esta sintaxe acima mostra algumas maneiras comuns de criar as instâncias de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="170d9-162">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="170d9-163">Todas as outras sintaxes POST que permitem criar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="170d9-163">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="170d9-164">Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="170d9-164">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="170d9-165">Crie uma extensão em uma instância de recurso existente</span><span class="sxs-lookup"><span data-stu-id="170d9-165">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="170d9-166">Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.</span><span class="sxs-lookup"><span data-stu-id="170d9-166">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="170d9-p103">**Observação:** Esta sintaxe mostra algumas maneiras comuns de identificar uma instância de recurso, a fim de criar uma extensão nele. Todas as outras sintaxes que permitem identificar essas instâncias de recursos suportam a criação de extensões abertas nelas de forma semelhante.</span><span class="sxs-lookup"><span data-stu-id="170d9-p103">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="170d9-169">Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="170d9-169">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="170d9-170">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="170d9-170">Path parameters</span></span>
|<span data-ttu-id="170d9-171">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="170d9-171">Parameter</span></span>|<span data-ttu-id="170d9-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="170d9-172">Type</span></span>|<span data-ttu-id="170d9-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="170d9-173">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="170d9-174">id</span><span class="sxs-lookup"><span data-stu-id="170d9-174">id</span></span>|<span data-ttu-id="170d9-175">string</span><span class="sxs-lookup"><span data-stu-id="170d9-175">string</span></span>|<span data-ttu-id="170d9-p104">Um identificador exclusivo para um objeto na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="170d9-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="170d9-178">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="170d9-178">Request headers</span></span>

| <span data-ttu-id="170d9-179">Nome</span><span class="sxs-lookup"><span data-stu-id="170d9-179">Name</span></span>       | <span data-ttu-id="170d9-180">Valor</span><span class="sxs-lookup"><span data-stu-id="170d9-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="170d9-181">Autorização</span><span class="sxs-lookup"><span data-stu-id="170d9-181">Authorization</span></span> | <span data-ttu-id="170d9-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="170d9-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="170d9-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="170d9-184">Content-Type</span></span> | <span data-ttu-id="170d9-185">application/json</span><span class="sxs-lookup"><span data-stu-id="170d9-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="170d9-186">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="170d9-186">Request body</span></span>

<span data-ttu-id="170d9-p106">Forneça um corpo JSON de uma [openTypeExtension](../resources/opentypeextension.md), com os seguintes pares de nome/valor obrigatórios e dados personalizados adicionais. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="170d9-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="170d9-189">Name</span><span class="sxs-lookup"><span data-stu-id="170d9-189">Name</span></span>       | <span data-ttu-id="170d9-190">Valor</span><span class="sxs-lookup"><span data-stu-id="170d9-190">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="170d9-191">@odata.type</span><span class="sxs-lookup"><span data-stu-id="170d9-191">@odata.type</span></span> | <span data-ttu-id="170d9-192">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="170d9-192">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="170d9-193">extensionName</span><span class="sxs-lookup"><span data-stu-id="170d9-193">extensionName</span></span> | <span data-ttu-id="170d9-194">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="170d9-194">%unique_string%</span></span> |

<span data-ttu-id="170d9-195">Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.</span><span class="sxs-lookup"><span data-stu-id="170d9-195">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="170d9-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="170d9-196">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="170d9-197">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="170d9-197">Response code</span></span>

<span data-ttu-id="170d9-198">Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="170d9-198">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="170d9-p107">Quando você cria uma extensão usando a mesma operação que você usa para criar uma instância de recurso, a operação retorna o mesmo código de resposta retornado quando você usa a operação para criar a instância de recurso sem a extensão. Consulte os tópicos correspondentes para a criação da instância, conforme listado [acima](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="170d9-p107">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension. Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="170d9-201">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="170d9-201">Response body</span></span>

| <span data-ttu-id="170d9-202">Cenário</span><span class="sxs-lookup"><span data-stu-id="170d9-202">Scenario</span></span>       | <span data-ttu-id="170d9-203">Recurso</span><span class="sxs-lookup"><span data-stu-id="170d9-203">Resource</span></span>  | <span data-ttu-id="170d9-204">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="170d9-204">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="170d9-205">Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso</span><span class="sxs-lookup"><span data-stu-id="170d9-205">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="170d9-206">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="170d9-206">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="170d9-207">Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="170d9-207">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="170d9-208">Criando uma extensão ao criar implicitamente uma instância de recursos</span><span class="sxs-lookup"><span data-stu-id="170d9-208">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="170d9-209">postagem</span><span class="sxs-lookup"><span data-stu-id="170d9-209">post</span></span>](../resources/post.md) | <span data-ttu-id="170d9-210">A resposta inclui somente um código de resposta, mas não um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="170d9-210">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="170d9-211">Criar uma extensão em uma instância de recurso _existente_</span><span class="sxs-lookup"><span data-stu-id="170d9-211">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="170d9-212">Todos os recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="170d9-212">All supported resources</span></span> | <span data-ttu-id="170d9-213">Inclui o objeto **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="170d9-213">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="170d9-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="170d9-214">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="170d9-215">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="170d9-215">Request 1</span></span>

<span data-ttu-id="170d9-p108">O primeiro exemplo cria uma mensagem e uma extensão na mesma chamada. O corpo da solicitação inclui o seguinte:</span><span class="sxs-lookup"><span data-stu-id="170d9-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="170d9-218">As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="170d9-218">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="170d9-219">E para a extensão:</span><span class="sxs-lookup"><span data-stu-id="170d9-219">And for the extension:</span></span>

  - <span data-ttu-id="170d9-220">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="170d9-220">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="170d9-221">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="170d9-221">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="170d9-222">Dados adicionais a serem armazenados como três propriedades personalizadas no conteúdo JSON: `companyName`, `expirationDate` e `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="170d9-222">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>


# <a name="http"></a>[<span data-ttu-id="170d9-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="170d9-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="170d9-224">C#</span><span class="sxs-lookup"><span data-stu-id="170d9-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="170d9-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="170d9-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="170d9-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="170d9-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="170d9-227">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="170d9-227">Response 1</span></span>

<span data-ttu-id="170d9-p109">Veja a seguir a resposta para o primeiro exemplo. O corpo da resposta inclui propriedades da nova mensagem e o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="170d9-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="170d9-230">A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="170d9-230">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="170d9-231">A propriedade padrão **extensionName** especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="170d9-231">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="170d9-232">Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="170d9-232">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="170d9-233">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="170d9-233">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="request-2"></a><span data-ttu-id="170d9-234">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="170d9-234">Request 2</span></span>

<span data-ttu-id="170d9-p110">O segundo exemplo cria uma extensão na mensagem especificada. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="170d9-p110">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="170d9-237">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="170d9-237">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="170d9-238">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="170d9-238">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="170d9-239">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="170d9-239">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="170d9-240">HTTP</span><span class="sxs-lookup"><span data-stu-id="170d9-240">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="170d9-241">C#</span><span class="sxs-lookup"><span data-stu-id="170d9-241">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="170d9-242">JavaScript</span><span class="sxs-lookup"><span data-stu-id="170d9-242">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="170d9-243">Objective-C</span><span class="sxs-lookup"><span data-stu-id="170d9-243">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="170d9-244">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="170d9-244">Response 2</span></span>

<span data-ttu-id="170d9-p111">Veja a seguir a resposta para o segundo exemplo. O corpo da solicitação inclui o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="170d9-p111">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="170d9-247">A propriedade padrão **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="170d9-247">The default property **extensionName**.</span></span>
- <span data-ttu-id="170d9-248">A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="170d9-248">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="170d9-249">Os dados personalizados a serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="170d9-249">The custom data to be stored.</span></span>

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

### <a name="request-3"></a><span data-ttu-id="170d9-250">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="170d9-250">Request 3</span></span>

<span data-ttu-id="170d9-p112">O terceiro exemplo cria uma extensão no evento de grupo especificado. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="170d9-p112">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="170d9-253">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="170d9-253">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="170d9-254">O nome da extensão "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="170d9-254">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="170d9-255">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="170d9-255">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="170d9-256">HTTP</span><span class="sxs-lookup"><span data-stu-id="170d9-256">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="170d9-257">C#</span><span class="sxs-lookup"><span data-stu-id="170d9-257">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="170d9-258">JavaScript</span><span class="sxs-lookup"><span data-stu-id="170d9-258">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="170d9-259">Objective-C</span><span class="sxs-lookup"><span data-stu-id="170d9-259">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="170d9-260">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="170d9-260">Response 3</span></span>

<span data-ttu-id="170d9-261">Veja a seguir a resposta da terceira solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="170d9-261">Here is the response from the third example request.</span></span>

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

### <a name="request-4"></a><span data-ttu-id="170d9-262">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="170d9-262">Request 4</span></span>

<span data-ttu-id="170d9-p113">O quarto exemplo cria uma extensão em uma nova postagem de grupo, usando a mesma chamada de ação **reply** para uma postagem de grupo existente. A ação **reply** cria uma nova postagem e uma nova extensão inserida nessa postagem. O corpo da solicitação inclui uma propriedade **post** que, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="170d9-p113">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="170d9-266">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="170d9-266">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="170d9-267">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="170d9-267">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="170d9-268">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="170d9-268">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="170d9-269">HTTP</span><span class="sxs-lookup"><span data-stu-id="170d9-269">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="170d9-270">C#</span><span class="sxs-lookup"><span data-stu-id="170d9-270">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="170d9-271">JavaScript</span><span class="sxs-lookup"><span data-stu-id="170d9-271">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="170d9-272">Objective-C</span><span class="sxs-lookup"><span data-stu-id="170d9-272">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-4"></a><span data-ttu-id="170d9-273">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="170d9-273">Response 4</span></span>

<span data-ttu-id="170d9-p114">Veja a seguir a resposta do quarto exemplo. Criar uma extensão com êxito em uma nova postagem de grupo resulta apenas no código de resposta HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="170d9-p114">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="170d9-276">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="170d9-276">Request 5</span></span>

<span data-ttu-id="170d9-p115">O quinto exemplo cria uma extensão em uma nova postagem de grupo usando a mesma operação POST para criar uma conversa. A operação POST cria uma nova conversa, thread ou postagem e uma nova extensão inserida na postagem. O corpo da solicitação inclui as propriedades **Topic** e **Threads** e o objeto filho **post** para a nova conversa. O objeto **post**, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a extensão:</span><span class="sxs-lookup"><span data-stu-id="170d9-p115">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="170d9-281">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="170d9-281">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="170d9-282">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="170d9-282">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="170d9-283">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="170d9-283">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="170d9-284">HTTP</span><span class="sxs-lookup"><span data-stu-id="170d9-284">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="170d9-285">C#</span><span class="sxs-lookup"><span data-stu-id="170d9-285">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="170d9-286">JavaScript</span><span class="sxs-lookup"><span data-stu-id="170d9-286">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="170d9-287">Objective-C</span><span class="sxs-lookup"><span data-stu-id="170d9-287">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-5"></a><span data-ttu-id="170d9-288">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="170d9-288">Response 5</span></span>

<span data-ttu-id="170d9-p116">Veja a seguir a resposta do quinto exemplo, que contém a nova conversa e uma ID de thread. Esse novo thread contém uma postagem criada automaticamente que, por sua vez, contém a nova extensão.</span><span class="sxs-lookup"><span data-stu-id="170d9-p116">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="170d9-291">Observação: O objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="170d9-291">Note: The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="170d9-p117">Para obter a nova extensão, primeiro [obtenha todas as postagens](../api/conversationthread-list-posts.md) desse thread. Inicialmente, deve haver somente uma. Em seguida, aplique a ID da postagem e o nome da extensão `Com.Contoso.Benefits` para [obter a extensão](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="170d9-p117">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

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

