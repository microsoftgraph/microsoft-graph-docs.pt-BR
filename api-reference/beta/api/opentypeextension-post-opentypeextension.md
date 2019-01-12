---
title: Criar extensão aberta
description: Criar uma extensão aberta (objeto openTypeExtension) e adicionar propriedades personalizadas
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 58df4ab2898abe0e49563de4b655eccacfdc91fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948566"
---
# <a name="create-open-extension"></a><span data-ttu-id="ddb32-103">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="ddb32-103">Create open extension</span></span>

> <span data-ttu-id="ddb32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ddb32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddb32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ddb32-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddb32-106">Crie uma extensão aberta (objeto[openTypeExtension](../resources/opentypeextension.md) ) e adicionar propriedades personalizadas em uma instância de um recurso com suporte do nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="ddb32-106">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="ddb32-107">**Observação:** Se você estiver criando extensões open nos recursos do Outlook, consulte **Considerações específicas do Outlook** em [tipo de recurso openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="ddb32-107">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddb32-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="ddb32-108">Permissions</span></span>

<span data-ttu-id="ddb32-109">Dependendo do recurso que você está criando a extensão na e a permissão tipo (delegado ou aplicativo) solicitada, a permissão especificada na tabela a seguir é o menos privilegiada necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ddb32-109">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="ddb32-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb32-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddb32-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-111">Supported resource</span></span> | <span data-ttu-id="ddb32-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddb32-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ddb32-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddb32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddb32-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddb32-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="ddb32-115">device</span><span class="sxs-lookup"><span data-stu-id="ddb32-115">device</span></span>](../resources/device.md) | <span data-ttu-id="ddb32-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="ddb32-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-117">Not supported</span></span> | <span data-ttu-id="ddb32-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="ddb32-119">evento</span><span class="sxs-lookup"><span data-stu-id="ddb32-119">event</span></span>](../resources/event.md) | <span data-ttu-id="ddb32-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="ddb32-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="ddb32-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="ddb32-123">grupo</span><span class="sxs-lookup"><span data-stu-id="ddb32-123">group</span></span>](../resources/group.md) | <span data-ttu-id="ddb32-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="ddb32-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-125">Not supported</span></span> | <span data-ttu-id="ddb32-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="ddb32-127">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="ddb32-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="ddb32-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="ddb32-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-129">Not supported</span></span> | <span data-ttu-id="ddb32-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-130">Not supported</span></span> |
| [<span data-ttu-id="ddb32-131">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="ddb32-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="ddb32-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="ddb32-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-133">Not supported</span></span> | <span data-ttu-id="ddb32-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="ddb32-135">mensagem</span><span class="sxs-lookup"><span data-stu-id="ddb32-135">message</span></span>](../resources/message.md) | <span data-ttu-id="ddb32-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-136">Mail.ReadWrite</span></span> | <span data-ttu-id="ddb32-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-137">Mail.ReadWrite</span></span> | <span data-ttu-id="ddb32-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="ddb32-139">organização</span><span class="sxs-lookup"><span data-stu-id="ddb32-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="ddb32-140">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-140">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="ddb32-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-141">Not supported</span></span> | <span data-ttu-id="ddb32-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-142">Not supported</span></span> |
| [<span data-ttu-id="ddb32-143">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="ddb32-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="ddb32-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="ddb32-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="ddb32-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="ddb32-147">usuário</span><span class="sxs-lookup"><span data-stu-id="ddb32-147">user</span></span>](../resources/user.md) | <span data-ttu-id="ddb32-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-148">User.ReadWrite.All</span></span> | <span data-ttu-id="ddb32-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb32-149">User.ReadWrite</span></span> | <span data-ttu-id="ddb32-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb32-150">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddb32-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb32-151">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="ddb32-152">Crie uma extensão em uma nova instância de recurso</span><span class="sxs-lookup"><span data-stu-id="ddb32-152">Create an extension in a new resource instance</span></span>

<span data-ttu-id="ddb32-153">Use a mesma solicitação REST que você usa para criar a instância.</span><span class="sxs-lookup"><span data-stu-id="ddb32-153">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="ddb32-154">**Observação:** Esta sintaxe mostra algumas maneiras comuns de criar as instâncias de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="ddb32-154">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="ddb32-155">Todas as outras sintaxes POST que permite que você crie essas instâncias de recurso suporta as extensões de open criação de forma semelhante.</span><span class="sxs-lookup"><span data-stu-id="ddb32-155">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="ddb32-156">Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddb32-156">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="ddb32-157">Crie uma extensão em uma instância de recurso existente</span><span class="sxs-lookup"><span data-stu-id="ddb32-157">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="ddb32-158">Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.</span><span class="sxs-lookup"><span data-stu-id="ddb32-158">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="ddb32-159">**Observação:** Esta sintaxe mostra algumas maneiras comuns de identificar uma instância de recurso, para criar uma extensão nela.</span><span class="sxs-lookup"><span data-stu-id="ddb32-159">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="ddb32-160">Oferece suporte a todas as outras sintaxes que permite que você identifique essas instâncias de recurso, Criando extensões open de forma semelhante.</span><span class="sxs-lookup"><span data-stu-id="ddb32-160">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="ddb32-161">Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddb32-161">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="ddb32-162">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="ddb32-162">Path parameters</span></span>

|<span data-ttu-id="ddb32-163">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="ddb32-163">**Parameter**</span></span>|<span data-ttu-id="ddb32-164">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="ddb32-164">**Type**</span></span>|<span data-ttu-id="ddb32-165">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ddb32-165">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ddb32-166">id</span><span class="sxs-lookup"><span data-stu-id="ddb32-166">id</span></span>|<span data-ttu-id="ddb32-167">string</span><span class="sxs-lookup"><span data-stu-id="ddb32-167">string</span></span>|<span data-ttu-id="ddb32-p105">Um identificador exclusivo para um objeto na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddb32-p105">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ddb32-170">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb32-170">Request headers</span></span>

| <span data-ttu-id="ddb32-171">Nome</span><span class="sxs-lookup"><span data-stu-id="ddb32-171">Name</span></span>       | <span data-ttu-id="ddb32-172">Valor</span><span class="sxs-lookup"><span data-stu-id="ddb32-172">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ddb32-173">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddb32-173">Authorization</span></span> | <span data-ttu-id="ddb32-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddb32-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddb32-176">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ddb32-176">Content-Type</span></span> | <span data-ttu-id="ddb32-177">application/json</span><span class="sxs-lookup"><span data-stu-id="ddb32-177">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddb32-178">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb32-178">Request body</span></span>

<span data-ttu-id="ddb32-179">Fornecer um corpo JSON de uma [openTypeExtension](../resources/opentypeextension.md), com os seguintes pares nome-valor necessários e quaisquer dados personalizados adicionais.</span><span class="sxs-lookup"><span data-stu-id="ddb32-179">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span></span> <span data-ttu-id="ddb32-180">Os dados na carga JSON podem ser primitivos tipos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="ddb32-180">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="ddb32-181">Nome</span><span class="sxs-lookup"><span data-stu-id="ddb32-181">Name</span></span>       | <span data-ttu-id="ddb32-182">Valor</span><span class="sxs-lookup"><span data-stu-id="ddb32-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ddb32-183">@odata.type</span><span class="sxs-lookup"><span data-stu-id="ddb32-183">@odata.type</span></span> | <span data-ttu-id="ddb32-184">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="ddb32-184">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="ddb32-185">extensionName</span><span class="sxs-lookup"><span data-stu-id="ddb32-185">extensionName</span></span> | <span data-ttu-id="ddb32-186">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="ddb32-186">%unique_string%</span></span> |

<span data-ttu-id="ddb32-187">Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.</span><span class="sxs-lookup"><span data-stu-id="ddb32-187">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="ddb32-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb32-188">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="ddb32-189">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="ddb32-189">Response code</span></span>

<span data-ttu-id="ddb32-190">Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-190">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="ddb32-191">Quando você cria uma extensão usando a mesma operação que você pode usar para criar uma instância de recurso, a operação retorna o código de resposta mesmo que ele retorna ao usar a operação para criar a instância de recurso sem a extensão.</span><span class="sxs-lookup"><span data-stu-id="ddb32-191">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="ddb32-192">Consulte os tópicos correspondentes para criar a instância, como listadas [acima](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="ddb32-192">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="ddb32-193">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="ddb32-193">Response body</span></span>

| <span data-ttu-id="ddb32-194">Cenário</span><span class="sxs-lookup"><span data-stu-id="ddb32-194">Scenario</span></span>       | <span data-ttu-id="ddb32-195">Recurso</span><span class="sxs-lookup"><span data-stu-id="ddb32-195">Resource</span></span>  | <span data-ttu-id="ddb32-196">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="ddb32-196">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="ddb32-197">Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso</span><span class="sxs-lookup"><span data-stu-id="ddb32-197">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="ddb32-198">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="ddb32-198">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="ddb32-199">Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="ddb32-199">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="ddb32-200">Criando uma extensão ao criar implicitamente uma instância de recursos</span><span class="sxs-lookup"><span data-stu-id="ddb32-200">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="ddb32-201">postagem</span><span class="sxs-lookup"><span data-stu-id="ddb32-201">post</span></span>](../resources/post.md) | <span data-ttu-id="ddb32-202">A resposta inclui somente um código de resposta, mas não um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb32-202">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="ddb32-203">Criar uma extensão em uma instância de recurso _existente_</span><span class="sxs-lookup"><span data-stu-id="ddb32-203">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="ddb32-204">Todos os recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="ddb32-204">All supported resources</span></span> | <span data-ttu-id="ddb32-205">Inclui o objeto **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="ddb32-205">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="ddb32-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddb32-206">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="ddb32-207">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="ddb32-207">Request 1</span></span>

<span data-ttu-id="ddb32-p109">O primeiro exemplo cria uma mensagem e uma extensão na mesma chamada. O corpo da solicitação inclui o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ddb32-p109">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="ddb32-210">As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="ddb32-210">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="ddb32-211">E para a extensão:</span><span class="sxs-lookup"><span data-stu-id="ddb32-211">And for the extension:</span></span>

  - <span data-ttu-id="ddb32-212">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-212">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
  - <span data-ttu-id="ddb32-213">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="ddb32-213">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="ddb32-214">Dados adicionais a serem armazenados como três propriedades personalizadas na carga JSON: `companyName`, `expirationDate`, e `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-214">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages

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
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="ddb32-215">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="ddb32-215">Response 1</span></span>

<span data-ttu-id="ddb32-p110">Veja a seguir a resposta para o primeiro exemplo. O corpo da resposta inclui propriedades da nova mensagem e o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="ddb32-p110">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="ddb32-218">A propriedade **id** com o nome totalmente qualificado de `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-218">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="ddb32-219">A propriedade padrão **extensionName** especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddb32-219">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="ddb32-220">Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="ddb32-220">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="ddb32-p111">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddb32-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="ddb32-223">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="ddb32-223">Request 2</span></span>

<span data-ttu-id="ddb32-p112">O segundo exemplo cria uma extensão na mensagem especificada. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="ddb32-p112">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="ddb32-226">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-226">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="ddb32-227">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="ddb32-227">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="ddb32-228">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-228">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="ddb32-229">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="ddb32-229">Response 2</span></span>

<span data-ttu-id="ddb32-p113">Veja a seguir a resposta para o segundo exemplo. O corpo da solicitação inclui o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="ddb32-p113">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="ddb32-232">A propriedade padrão **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="ddb32-232">The default property **extensionName**.</span></span>
- <span data-ttu-id="ddb32-233">A propriedade **id** com o nome totalmente qualificado de `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-233">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="ddb32-234">Os dados personalizados a serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="ddb32-234">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="ddb32-235">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="ddb32-235">Request 3</span></span>

<span data-ttu-id="ddb32-p114">O terceiro exemplo cria uma extensão no evento de grupo especificado. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="ddb32-p114">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="ddb32-238">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-238">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="ddb32-239">O nome da extensão "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="ddb32-239">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="ddb32-240">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-240">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="ddb32-241">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="ddb32-241">Response 3</span></span>

<span data-ttu-id="ddb32-242">Veja a seguir a resposta da terceira solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="ddb32-242">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="ddb32-243">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="ddb32-243">Request 4</span></span>

<span data-ttu-id="ddb32-p115">O quarto exemplo cria uma extensão em uma nova postagem de grupo, usando a mesma chamada de ação **reply** para uma postagem de grupo existente. A ação **reply** cria uma nova postagem e uma nova extensão inserida nessa postagem. O corpo da solicitação inclui uma propriedade **post** que, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="ddb32-p115">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="ddb32-247">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-247">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="ddb32-248">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="ddb32-248">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="ddb32-249">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-249">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
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

### <a name="response-4"></a><span data-ttu-id="ddb32-250">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="ddb32-250">Response 4</span></span>

<span data-ttu-id="ddb32-p116">Veja a seguir a resposta do quarto exemplo. Criar uma extensão com êxito em uma nova postagem de grupo resulta apenas no código de resposta HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="ddb32-p116">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="ddb32-253">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="ddb32-253">Request 5</span></span>

<span data-ttu-id="ddb32-p117">O quinto exemplo cria uma extensão em uma nova postagem de grupo usando a mesma operação POST para criar uma conversa. A operação POST cria uma nova conversa, thread ou postagem e uma nova extensão inserida na postagem. O corpo da solicitação inclui as propriedades **Topic** e **Threads** e o objeto filho **post** para a nova conversa. O objeto **post**, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a extensão:</span><span class="sxs-lookup"><span data-stu-id="ddb32-p117">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="ddb32-258">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-258">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="ddb32-259">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="ddb32-259">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="ddb32-260">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="ddb32-260">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

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
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
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

### <a name="response-5"></a><span data-ttu-id="ddb32-261">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="ddb32-261">Response 5</span></span>

<span data-ttu-id="ddb32-p118">Veja a seguir a resposta do quinto exemplo, que contém a nova conversa e uma ID de thread. Esse novo thread contém uma postagem criada automaticamente que, por sua vez, contém a nova extensão.</span><span class="sxs-lookup"><span data-stu-id="ddb32-p118">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="ddb32-p119">Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddb32-p119">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="ddb32-p120">Para obter a nova extensão, primeiro [obtenha todas as postagens](../api/conversationthread-list-posts.md) desse thread. Inicialmente, deve haver somente uma. Em seguida, aplique a ID da postagem e o nome da extensão `Com.Contoso.Benefits` para [obter a extensão](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="ddb32-p120">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
