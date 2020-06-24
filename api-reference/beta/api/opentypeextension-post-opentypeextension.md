---
title: Criar extensão aberta
description: Criar uma extensão aberta (objeto openTypeExtension) e adicionar propriedades personalizadas
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: d6c06370494e9e89fa77d40a0889819f47f21d2c
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863366"
---
# <a name="create-open-extension"></a><span data-ttu-id="4a988-103">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="4a988-103">Create open extension</span></span>

<span data-ttu-id="4a988-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a988-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a988-105">Crie uma extensão aberta (objeto[openTypeExtension](../resources/opentypeextension.md) ) e adicione Propriedades personalizadas em uma instância nova ou existente de um recurso com suporte.</span><span class="sxs-lookup"><span data-stu-id="4a988-105">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="4a988-106">**Observação:** Se você estiver criando extensões abertas em recursos do Outlook, confira **considerações específicas do Outlook** no [tipo de recurso openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="4a988-106">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a988-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a988-107">Permissions</span></span>

<span data-ttu-id="4a988-108">Dependendo do recurso para o qual você está criando a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="4a988-108">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4a988-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a988-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a988-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="4a988-110">Supported resource</span></span> | <span data-ttu-id="4a988-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a988-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a988-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a988-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a988-113">Application</span><span class="sxs-lookup"><span data-stu-id="4a988-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="4a988-114">device</span><span class="sxs-lookup"><span data-stu-id="4a988-114">device</span></span>](../resources/device.md) | <span data-ttu-id="4a988-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a988-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="4a988-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4a988-116">Not supported</span></span> | <span data-ttu-id="4a988-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="4a988-118">evento</span><span class="sxs-lookup"><span data-stu-id="4a988-118">event</span></span>](../resources/event.md) | <span data-ttu-id="4a988-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="4a988-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="4a988-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="4a988-122">grupo</span><span class="sxs-lookup"><span data-stu-id="4a988-122">group</span></span>](../resources/group.md) | <span data-ttu-id="4a988-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="4a988-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4a988-124">Not supported</span></span> | <span data-ttu-id="4a988-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="4a988-126">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="4a988-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="4a988-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="4a988-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4a988-128">Not supported</span></span> | <span data-ttu-id="4a988-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4a988-129">Not supported</span></span> |
| [<span data-ttu-id="4a988-130">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="4a988-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="4a988-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="4a988-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4a988-132">Not supported</span></span> | <span data-ttu-id="4a988-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="4a988-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="4a988-134">message</span></span>](../resources/message.md) | <span data-ttu-id="4a988-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-135">Mail.ReadWrite</span></span> | <span data-ttu-id="4a988-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-136">Mail.ReadWrite</span></span> | <span data-ttu-id="4a988-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="4a988-138">organização</span><span class="sxs-lookup"><span data-stu-id="4a988-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="4a988-139">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-139">Organization.ReadWrite.All</span></span> | <span data-ttu-id="4a988-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4a988-140">Not supported</span></span> | <span data-ttu-id="4a988-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-141">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="4a988-142">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="4a988-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="4a988-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="4a988-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="4a988-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="4a988-146">user</span><span class="sxs-lookup"><span data-stu-id="4a988-146">user</span></span>](../resources/user.md) | <span data-ttu-id="4a988-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-147">User.ReadWrite</span></span> | <span data-ttu-id="4a988-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a988-148">User.ReadWrite</span></span> | <span data-ttu-id="4a988-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a988-149">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a988-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a988-150">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="4a988-151">Crie uma extensão em uma nova instância de recurso</span><span class="sxs-lookup"><span data-stu-id="4a988-151">Create an extension in a new resource instance</span></span>

<span data-ttu-id="4a988-152">Use a mesma solicitação REST usada para criar a instância.</span><span class="sxs-lookup"><span data-stu-id="4a988-152">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="4a988-153">**Observação:** Esta sintaxe acima mostra algumas maneiras comuns de criar as instâncias de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="4a988-153">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="4a988-154">Todas as outras sintaxes POST que permitem criar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="4a988-154">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="4a988-155">Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a988-155">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="4a988-156">Crie uma extensão em uma instância de recurso existente</span><span class="sxs-lookup"><span data-stu-id="4a988-156">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="4a988-157">Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.</span><span class="sxs-lookup"><span data-stu-id="4a988-157">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /administrativeunits/{id}/extensions
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="4a988-158">**Observação:** Esta sintaxe mostra algumas maneiras comuns de identificar uma instância do recurso, para criar uma extensão nele.</span><span class="sxs-lookup"><span data-stu-id="4a988-158">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="4a988-159">Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="4a988-159">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="4a988-160">Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a988-160">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="4a988-161">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="4a988-161">Path parameters</span></span>

|<span data-ttu-id="4a988-162">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="4a988-162">**Parameter**</span></span>|<span data-ttu-id="4a988-163">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="4a988-163">**Type**</span></span>|<span data-ttu-id="4a988-164">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4a988-164">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4a988-165">id</span><span class="sxs-lookup"><span data-stu-id="4a988-165">id</span></span>|<span data-ttu-id="4a988-166">string</span><span class="sxs-lookup"><span data-stu-id="4a988-166">string</span></span>|<span data-ttu-id="4a988-167">A unique identifier for an object in the corresponding collection.</span><span class="sxs-lookup"><span data-stu-id="4a988-167">A unique identifier for an object in the corresponding collection.</span></span> <span data-ttu-id="4a988-168">Required.</span><span class="sxs-lookup"><span data-stu-id="4a988-168">Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4a988-169">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a988-169">Request headers</span></span>

| <span data-ttu-id="4a988-170">Nome</span><span class="sxs-lookup"><span data-stu-id="4a988-170">Name</span></span>       | <span data-ttu-id="4a988-171">Valor</span><span class="sxs-lookup"><span data-stu-id="4a988-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4a988-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a988-172">Authorization</span></span> | <span data-ttu-id="4a988-173">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4a988-173">Bearer {token}.</span></span> <span data-ttu-id="4a988-174">Required.</span><span class="sxs-lookup"><span data-stu-id="4a988-174">Required.</span></span> |
| <span data-ttu-id="4a988-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a988-175">Content-Type</span></span> | <span data-ttu-id="4a988-176">application/json</span><span class="sxs-lookup"><span data-stu-id="4a988-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a988-177">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a988-177">Request body</span></span>

<span data-ttu-id="4a988-178">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span><span class="sxs-lookup"><span data-stu-id="4a988-178">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span></span> <span data-ttu-id="4a988-179">The data in the JSON payload can be primitive types, or arrays of primitive types.</span><span class="sxs-lookup"><span data-stu-id="4a988-179">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="4a988-180">Name</span><span class="sxs-lookup"><span data-stu-id="4a988-180">Name</span></span>       | <span data-ttu-id="4a988-181">Valor</span><span class="sxs-lookup"><span data-stu-id="4a988-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4a988-182">@odata.type</span><span class="sxs-lookup"><span data-stu-id="4a988-182">@odata.type</span></span> | <span data-ttu-id="4a988-183">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="4a988-183">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="4a988-184">extensionName</span><span class="sxs-lookup"><span data-stu-id="4a988-184">extensionName</span></span> | <span data-ttu-id="4a988-185">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="4a988-185">%unique_string%</span></span> |

<span data-ttu-id="4a988-186">Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.</span><span class="sxs-lookup"><span data-stu-id="4a988-186">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="4a988-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a988-187">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="4a988-188">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="4a988-188">Response code</span></span>

<span data-ttu-id="4a988-189">Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="4a988-189">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="4a988-190">Quando você cria uma extensão usando a mesma operação usada para criar uma instância de recurso, a operação retorna o mesmo código de resposta retornado quando você usa a operação para criar a instância do recurso sem a extensão.</span><span class="sxs-lookup"><span data-stu-id="4a988-190">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="4a988-191">Consulte os tópicos correspondentes para criar a instância conforme listado [cima](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="4a988-191">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="4a988-192">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="4a988-192">Response body</span></span>

| <span data-ttu-id="4a988-193">Cenário</span><span class="sxs-lookup"><span data-stu-id="4a988-193">Scenario</span></span>       | <span data-ttu-id="4a988-194">Recurso</span><span class="sxs-lookup"><span data-stu-id="4a988-194">Resource</span></span>  | <span data-ttu-id="4a988-195">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="4a988-195">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="4a988-196">Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso</span><span class="sxs-lookup"><span data-stu-id="4a988-196">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="4a988-197">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="4a988-197">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="4a988-198">Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="4a988-198">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="4a988-199">Criando uma extensão ao criar implicitamente uma instância de recursos</span><span class="sxs-lookup"><span data-stu-id="4a988-199">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="4a988-200">postagem</span><span class="sxs-lookup"><span data-stu-id="4a988-200">post</span></span>](../resources/post.md) | <span data-ttu-id="4a988-201">A resposta inclui somente um código de resposta, mas não um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a988-201">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="4a988-202">Criar uma extensão em uma instância de recurso _existente_</span><span class="sxs-lookup"><span data-stu-id="4a988-202">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="4a988-203">Todos os recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="4a988-203">All supported resources</span></span> | <span data-ttu-id="4a988-204">Inclui o objeto **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="4a988-204">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="4a988-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a988-205">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="4a988-206">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="4a988-206">Request 1</span></span>

<span data-ttu-id="4a988-207">The first example creates a message and an extension in the same call.</span><span class="sxs-lookup"><span data-stu-id="4a988-207">The first example creates a message and an extension in the same call.</span></span> <span data-ttu-id="4a988-208">The request body includes the following:</span><span class="sxs-lookup"><span data-stu-id="4a988-208">The request body includes the following:</span></span>

- <span data-ttu-id="4a988-209">As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="4a988-209">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="4a988-210">E para a extensão:</span><span class="sxs-lookup"><span data-stu-id="4a988-210">And for the extension:</span></span>

  - <span data-ttu-id="4a988-211">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="4a988-211">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="4a988-212">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="4a988-212">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="4a988-213">Dados adicionais a serem armazenados como três propriedades personalizadas no conteúdo JSON: `companyName`, `expirationDate` e `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="4a988-213">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a988-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a988-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-Type: application/json

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
# <a name="c"></a>[<span data-ttu-id="4a988-215">C#</span><span class="sxs-lookup"><span data-stu-id="4a988-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a988-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a988-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a988-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a988-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="4a988-218">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="4a988-218">Response 1</span></span>

<span data-ttu-id="4a988-219">Here is the response for the first example.</span><span class="sxs-lookup"><span data-stu-id="4a988-219">Here is the response for the first example.</span></span> <span data-ttu-id="4a988-220">The response body includes properties of the new message, and the following for the new extension:</span><span class="sxs-lookup"><span data-stu-id="4a988-220">The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="4a988-221">A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="4a988-221">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="4a988-222">A propriedade padrão **extensionName** especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a988-222">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="4a988-223">Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="4a988-223">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="4a988-224">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="4a988-224">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4a988-225">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4a988-225">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
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
  "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
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

### <a name="request-2"></a><span data-ttu-id="4a988-226">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="4a988-226">Request 2</span></span>

<span data-ttu-id="4a988-227">The second example creates an extension in the specified message.</span><span class="sxs-lookup"><span data-stu-id="4a988-227">The second example creates an extension in the specified message.</span></span> <span data-ttu-id="4a988-228">The request body includes the following for the extension:</span><span class="sxs-lookup"><span data-stu-id="4a988-228">The request body includes the following for the extension:</span></span>

- <span data-ttu-id="4a988-229">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="4a988-229">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="4a988-230">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="4a988-230">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="4a988-231">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="4a988-231">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a988-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a988-232">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions
Content-Type: application/json

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="4a988-233">C#</span><span class="sxs-lookup"><span data-stu-id="4a988-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a988-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a988-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a988-235">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a988-235">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="4a988-236">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="4a988-236">Response 2</span></span>

<span data-ttu-id="4a988-237">Here is the response for the second example.</span><span class="sxs-lookup"><span data-stu-id="4a988-237">Here is the response for the second example.</span></span> <span data-ttu-id="4a988-238">The response body includes the following for the new extension:</span><span class="sxs-lookup"><span data-stu-id="4a988-238">The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="4a988-239">A propriedade padrão **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="4a988-239">The default property **extensionName**.</span></span>
- <span data-ttu-id="4a988-240">A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="4a988-240">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="4a988-241">Os dados personalizados a serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="4a988-241">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="4a988-242">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="4a988-242">Request 3</span></span>

<span data-ttu-id="4a988-243">The third example creates an extension in the specified group event.</span><span class="sxs-lookup"><span data-stu-id="4a988-243">The third example creates an extension in the specified group event.</span></span> <span data-ttu-id="4a988-244">The request body includes the following for the extension:</span><span class="sxs-lookup"><span data-stu-id="4a988-244">The request body includes the following for the extension:</span></span>

- <span data-ttu-id="4a988-245">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="4a988-245">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="4a988-246">O nome da extensão "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="4a988-246">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="4a988-247">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="4a988-247">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a988-248">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a988-248">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions
Content-type: application/json

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="4a988-249">C#</span><span class="sxs-lookup"><span data-stu-id="4a988-249">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a988-250">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a988-250">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a988-251">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a988-251">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="4a988-252">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="4a988-252">Response 3</span></span>

<span data-ttu-id="4a988-253">Veja a seguir a resposta da terceira solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="4a988-253">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="4a988-254">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="4a988-254">Request 4</span></span>

<span data-ttu-id="4a988-255">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post.</span><span class="sxs-lookup"><span data-stu-id="4a988-255">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post.</span></span> <span data-ttu-id="4a988-256">The **reply** action creates a new post, and a new extension embedded in the post.</span><span class="sxs-lookup"><span data-stu-id="4a988-256">The **reply** action creates a new post, and a new extension embedded in the post.</span></span> <span data-ttu-id="4a988-257">The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span><span class="sxs-lookup"><span data-stu-id="4a988-257">The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="4a988-258">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="4a988-258">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="4a988-259">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="4a988-259">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="4a988-260">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="4a988-260">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a988-261">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a988-261">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply
Content-type: application/json

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
# <a name="c"></a>[<span data-ttu-id="4a988-262">C#</span><span class="sxs-lookup"><span data-stu-id="4a988-262">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a988-263">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a988-263">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a988-264">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a988-264">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-4"></a><span data-ttu-id="4a988-265">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="4a988-265">Response 4</span></span>

<span data-ttu-id="4a988-266">Here is the response from the fourth example.</span><span class="sxs-lookup"><span data-stu-id="4a988-266">Here is the response from the fourth example.</span></span> <span data-ttu-id="4a988-267">Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span><span class="sxs-lookup"><span data-stu-id="4a988-267">Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="4a988-268">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="4a988-268">Request 5</span></span>

<span data-ttu-id="4a988-269">The fifth example creates an extension in a new group post using the same POST operation to create a conversation.</span><span class="sxs-lookup"><span data-stu-id="4a988-269">The fifth example creates an extension in a new group post using the same POST operation to create a conversation.</span></span> <span data-ttu-id="4a988-270">The POST operation creates a new conversation, thread and post, and a new extension embedded in the post.</span><span class="sxs-lookup"><span data-stu-id="4a988-270">The POST operation creates a new conversation, thread and post, and a new extension embedded in the post.</span></span> <span data-ttu-id="4a988-271">The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation.</span><span class="sxs-lookup"><span data-stu-id="4a988-271">The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation.</span></span> <span data-ttu-id="4a988-272">The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span><span class="sxs-lookup"><span data-stu-id="4a988-272">The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="4a988-273">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="4a988-273">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="4a988-274">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="4a988-274">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="4a988-275">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="4a988-275">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a988-276">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a988-276">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations
Content-type: application/json

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
# <a name="c"></a>[<span data-ttu-id="4a988-277">C#</span><span class="sxs-lookup"><span data-stu-id="4a988-277">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a988-278">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a988-278">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a988-279">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a988-279">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-5"></a><span data-ttu-id="4a988-280">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="4a988-280">Response 5</span></span>

<span data-ttu-id="4a988-281">Here is the response from the fifth example which contains the new conversation and a thread ID.</span><span class="sxs-lookup"><span data-stu-id="4a988-281">Here is the response from the fifth example which contains the new conversation and a thread ID.</span></span> <span data-ttu-id="4a988-282">This new thread contains an automatically created post, which in turn contains the new extension.</span><span class="sxs-lookup"><span data-stu-id="4a988-282">This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="4a988-283">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="4a988-283">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4a988-284">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4a988-284">All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="4a988-285">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one.</span><span class="sxs-lookup"><span data-stu-id="4a988-285">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one.</span></span> <span data-ttu-id="4a988-286">Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="4a988-286">Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
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
<!--
{
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
