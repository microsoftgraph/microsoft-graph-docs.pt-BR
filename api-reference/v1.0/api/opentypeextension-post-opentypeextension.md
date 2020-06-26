---
title: Criar extensão aberta
description: Crie uma extensão aberta (objeto openTypeExtension) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: b6ddd4fea0262d1a00ace3ebf406b65e611f4985
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864032"
---
# <a name="create-open-extension"></a><span data-ttu-id="44999-103">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="44999-103">Create open extension</span></span>

<span data-ttu-id="44999-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44999-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44999-105">Crie uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="44999-105">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

> <span data-ttu-id="44999-106">**Observação:** Se você estiver criando extensões abertas em recursos do Outlook, confira **considerações específicas do Outlook** no [tipo de recurso openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="44999-106">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="44999-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="44999-107">Permissions</span></span>

<span data-ttu-id="44999-108">Dependendo do recurso para o qual você está criando a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="44999-108">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="44999-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44999-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44999-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="44999-110">Supported resource</span></span> | <span data-ttu-id="44999-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44999-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44999-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44999-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44999-113">Application</span><span class="sxs-lookup"><span data-stu-id="44999-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="44999-114">device</span><span class="sxs-lookup"><span data-stu-id="44999-114">device</span></span>](../resources/device.md) | <span data-ttu-id="44999-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44999-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="44999-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44999-116">Not supported</span></span> | <span data-ttu-id="44999-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="44999-118">evento</span><span class="sxs-lookup"><span data-stu-id="44999-118">event</span></span>](../resources/event.md) | <span data-ttu-id="44999-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="44999-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="44999-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="44999-122">grupo</span><span class="sxs-lookup"><span data-stu-id="44999-122">group</span></span>](../resources/group.md) | <span data-ttu-id="44999-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="44999-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44999-124">Not supported</span></span> | <span data-ttu-id="44999-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="44999-126">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="44999-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="44999-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="44999-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44999-128">Not supported</span></span> | <span data-ttu-id="44999-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44999-129">Not supported</span></span> |
| [<span data-ttu-id="44999-130">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="44999-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="44999-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="44999-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="44999-132">Not supported</span></span> | <span data-ttu-id="44999-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="44999-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="44999-134">message</span></span>](../resources/message.md) | <span data-ttu-id="44999-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-135">Mail.ReadWrite</span></span> | <span data-ttu-id="44999-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-136">Mail.ReadWrite</span></span> | <span data-ttu-id="44999-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="44999-138">organization</span><span class="sxs-lookup"><span data-stu-id="44999-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="44999-139">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-139">Organization.ReadWrite.All</span></span> | <span data-ttu-id="44999-140">Incompatível</span><span class="sxs-lookup"><span data-stu-id="44999-140">Not supported</span></span> | <span data-ttu-id="44999-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-141">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="44999-142">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="44999-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="44999-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="44999-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="44999-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="44999-146">user</span><span class="sxs-lookup"><span data-stu-id="44999-146">user</span></span>](../resources/user.md) | <span data-ttu-id="44999-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-147">User.ReadWrite</span></span> | <span data-ttu-id="44999-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44999-148">User.ReadWrite</span></span> | <span data-ttu-id="44999-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44999-149">User.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="44999-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44999-150">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="44999-151">Crie uma extensão em uma nova instância de recurso</span><span class="sxs-lookup"><span data-stu-id="44999-151">Create an extension in a new resource instance</span></span>

<span data-ttu-id="44999-152">Use a mesma solicitação REST usada para criar a instância.</span><span class="sxs-lookup"><span data-stu-id="44999-152">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="44999-153">**Observação:** Esta sintaxe acima mostra algumas maneiras comuns de criar as instâncias de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="44999-153">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="44999-154">Todas as outras sintaxes POST que permitem criar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="44999-154">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="44999-155">Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44999-155">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="44999-156">Crie uma extensão em uma instância de recurso existente</span><span class="sxs-lookup"><span data-stu-id="44999-156">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="44999-157">Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.</span><span class="sxs-lookup"><span data-stu-id="44999-157">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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
```

><span data-ttu-id="44999-158">**Observação:** Esta sintaxe mostra algumas maneiras comuns de identificar uma instância do recurso, para criar uma extensão nele.</span><span class="sxs-lookup"><span data-stu-id="44999-158">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="44999-159">Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="44999-159">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="44999-160">Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44999-160">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="44999-161">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="44999-161">Path parameters</span></span>
|<span data-ttu-id="44999-162">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="44999-162">Parameter</span></span>|<span data-ttu-id="44999-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="44999-163">Type</span></span>|<span data-ttu-id="44999-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="44999-164">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="44999-165">id</span><span class="sxs-lookup"><span data-stu-id="44999-165">id</span></span>|<span data-ttu-id="44999-166">string</span><span class="sxs-lookup"><span data-stu-id="44999-166">string</span></span>|<span data-ttu-id="44999-167">A unique identifier for an object in the corresponding collection.</span><span class="sxs-lookup"><span data-stu-id="44999-167">A unique identifier for an object in the corresponding collection.</span></span> <span data-ttu-id="44999-168">Required.</span><span class="sxs-lookup"><span data-stu-id="44999-168">Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="44999-169">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44999-169">Request headers</span></span>

| <span data-ttu-id="44999-170">Nome</span><span class="sxs-lookup"><span data-stu-id="44999-170">Name</span></span>       | <span data-ttu-id="44999-171">Valor</span><span class="sxs-lookup"><span data-stu-id="44999-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="44999-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="44999-172">Authorization</span></span> | <span data-ttu-id="44999-173">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="44999-173">Bearer {token}.</span></span> <span data-ttu-id="44999-174">Required.</span><span class="sxs-lookup"><span data-stu-id="44999-174">Required.</span></span> |
| <span data-ttu-id="44999-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44999-175">Content-Type</span></span> | <span data-ttu-id="44999-176">application/json</span><span class="sxs-lookup"><span data-stu-id="44999-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="44999-177">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44999-177">Request body</span></span>

<span data-ttu-id="44999-178">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs, and any additional custom data.</span><span class="sxs-lookup"><span data-stu-id="44999-178">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs, and any additional custom data.</span></span> <span data-ttu-id="44999-179">The data in the JSON payload can be primitive types, or arrays of primitive types.</span><span class="sxs-lookup"><span data-stu-id="44999-179">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="44999-180">Name</span><span class="sxs-lookup"><span data-stu-id="44999-180">Name</span></span>       | <span data-ttu-id="44999-181">Valor</span><span class="sxs-lookup"><span data-stu-id="44999-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="44999-182">@odata.type</span><span class="sxs-lookup"><span data-stu-id="44999-182">@odata.type</span></span> | <span data-ttu-id="44999-183">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="44999-183">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="44999-184">extensionName</span><span class="sxs-lookup"><span data-stu-id="44999-184">extensionName</span></span> | <span data-ttu-id="44999-185">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="44999-185">%unique_string%</span></span> |

<span data-ttu-id="44999-186">Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.</span><span class="sxs-lookup"><span data-stu-id="44999-186">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="44999-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="44999-187">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="44999-188">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="44999-188">Response code</span></span>

<span data-ttu-id="44999-189">Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="44999-189">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="44999-190">Quando você cria uma extensão usando a mesma operação usada para criar uma instância de recurso, a operação retorna o mesmo código de resposta retornado quando você usa a operação para criar a instância do recurso sem a extensão.</span><span class="sxs-lookup"><span data-stu-id="44999-190">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="44999-191">Consulte os tópicos correspondentes para criar a instância conforme listado [cima](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="44999-191">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="44999-192">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="44999-192">Response body</span></span>

| <span data-ttu-id="44999-193">Cenário</span><span class="sxs-lookup"><span data-stu-id="44999-193">Scenario</span></span>       | <span data-ttu-id="44999-194">Recurso</span><span class="sxs-lookup"><span data-stu-id="44999-194">Resource</span></span>  | <span data-ttu-id="44999-195">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="44999-195">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="44999-196">Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso</span><span class="sxs-lookup"><span data-stu-id="44999-196">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="44999-197">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="44999-197">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="44999-198">Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="44999-198">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="44999-199">Criando uma extensão ao criar implicitamente uma instância de recursos</span><span class="sxs-lookup"><span data-stu-id="44999-199">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="44999-200">postagem</span><span class="sxs-lookup"><span data-stu-id="44999-200">post</span></span>](../resources/post.md) | <span data-ttu-id="44999-201">A resposta inclui somente um código de resposta, mas não um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44999-201">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="44999-202">Criar uma extensão em uma instância de recurso _existente_</span><span class="sxs-lookup"><span data-stu-id="44999-202">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="44999-203">Todos os recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="44999-203">All supported resources</span></span> | <span data-ttu-id="44999-204">Inclui o objeto **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="44999-204">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="44999-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44999-205">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="44999-206">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="44999-206">Request 1</span></span>

<span data-ttu-id="44999-207">The first example creates a message and an extension in the same call.</span><span class="sxs-lookup"><span data-stu-id="44999-207">The first example creates a message and an extension in the same call.</span></span> <span data-ttu-id="44999-208">The request body includes the following:</span><span class="sxs-lookup"><span data-stu-id="44999-208">The request body includes the following:</span></span>

- <span data-ttu-id="44999-209">As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="44999-209">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="44999-210">E para a extensão:</span><span class="sxs-lookup"><span data-stu-id="44999-210">And for the extension:</span></span>

  - <span data-ttu-id="44999-211">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="44999-211">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="44999-212">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="44999-212">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="44999-213">Dados adicionais a serem armazenados como três propriedades personalizadas no conteúdo JSON: `companyName`, `expirationDate` e `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="44999-213">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

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

### <a name="response-1"></a><span data-ttu-id="44999-214">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="44999-214">Response 1</span></span>

<span data-ttu-id="44999-215">Here is the response for the first example.</span><span class="sxs-lookup"><span data-stu-id="44999-215">Here is the response for the first example.</span></span> <span data-ttu-id="44999-216">The response body includes properties of the new message, and the following for the new extension:</span><span class="sxs-lookup"><span data-stu-id="44999-216">The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="44999-217">A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="44999-217">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="44999-218">A propriedade padrão **extensionName** especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="44999-218">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="44999-219">Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="44999-219">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="44999-220">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="44999-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="44999-221">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="44999-221">All of the properties will be returned from an actual call.</span></span>
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

### <a name="request-2"></a><span data-ttu-id="44999-222">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="44999-222">Request 2</span></span>

<span data-ttu-id="44999-223">The second example creates an extension in the specified message.</span><span class="sxs-lookup"><span data-stu-id="44999-223">The second example creates an extension in the specified message.</span></span> <span data-ttu-id="44999-224">The request body includes the following for the extension:</span><span class="sxs-lookup"><span data-stu-id="44999-224">The request body includes the following for the extension:</span></span>

- <span data-ttu-id="44999-225">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="44999-225">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="44999-226">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="44999-226">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="44999-227">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="44999-227">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

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

### <a name="response-2"></a><span data-ttu-id="44999-228">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="44999-228">Response 2</span></span>

<span data-ttu-id="44999-229">Here is the response for the second example.</span><span class="sxs-lookup"><span data-stu-id="44999-229">Here is the response for the second example.</span></span> <span data-ttu-id="44999-230">The response body includes the following for the new extension:</span><span class="sxs-lookup"><span data-stu-id="44999-230">The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="44999-231">A propriedade padrão **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="44999-231">The default property **extensionName**.</span></span>
- <span data-ttu-id="44999-232">A propriedade **id** com o nome totalmente qualificado de `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="44999-232">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="44999-233">Os dados personalizados a serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="44999-233">The custom data to be stored.</span></span>

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

### <a name="request-3"></a><span data-ttu-id="44999-234">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="44999-234">Request 3</span></span>

<span data-ttu-id="44999-235">The third example creates an extension in the specified group event.</span><span class="sxs-lookup"><span data-stu-id="44999-235">The third example creates an extension in the specified group event.</span></span> <span data-ttu-id="44999-236">The request body includes the following for the extension:</span><span class="sxs-lookup"><span data-stu-id="44999-236">The request body includes the following for the extension:</span></span>

- <span data-ttu-id="44999-237">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="44999-237">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="44999-238">O nome da extensão "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="44999-238">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="44999-239">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="44999-239">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

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

### <a name="response-3"></a><span data-ttu-id="44999-240">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="44999-240">Response 3</span></span>

<span data-ttu-id="44999-241">Veja a seguir a resposta da terceira solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="44999-241">Here is the response from the third example request.</span></span>

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

### <a name="request-4"></a><span data-ttu-id="44999-242">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="44999-242">Request 4</span></span>

<span data-ttu-id="44999-243">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post.</span><span class="sxs-lookup"><span data-stu-id="44999-243">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post.</span></span> <span data-ttu-id="44999-244">The **reply** action creates a new post, and a new extension embedded in the post.</span><span class="sxs-lookup"><span data-stu-id="44999-244">The **reply** action creates a new post, and a new extension embedded in the post.</span></span> <span data-ttu-id="44999-245">The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span><span class="sxs-lookup"><span data-stu-id="44999-245">The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="44999-246">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="44999-246">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="44999-247">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="44999-247">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="44999-248">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="44999-248">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

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

### <a name="response-4"></a><span data-ttu-id="44999-249">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="44999-249">Response 4</span></span>

<span data-ttu-id="44999-250">Here is the response from the fourth example.</span><span class="sxs-lookup"><span data-stu-id="44999-250">Here is the response from the fourth example.</span></span> <span data-ttu-id="44999-251">Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span><span class="sxs-lookup"><span data-stu-id="44999-251">Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="44999-252">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="44999-252">Request 5</span></span>

<span data-ttu-id="44999-253">The fifth example creates an extension in a new group post using the same POST operation to create a conversation.</span><span class="sxs-lookup"><span data-stu-id="44999-253">The fifth example creates an extension in a new group post using the same POST operation to create a conversation.</span></span> <span data-ttu-id="44999-254">The POST operation creates a new conversation, thread and post, and a new extension embedded in the post.</span><span class="sxs-lookup"><span data-stu-id="44999-254">The POST operation creates a new conversation, thread and post, and a new extension embedded in the post.</span></span> <span data-ttu-id="44999-255">The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation.</span><span class="sxs-lookup"><span data-stu-id="44999-255">The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation.</span></span> <span data-ttu-id="44999-256">The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span><span class="sxs-lookup"><span data-stu-id="44999-256">The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="44999-257">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="44999-257">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="44999-258">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="44999-258">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="44999-259">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="44999-259">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

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

### <a name="response-5"></a><span data-ttu-id="44999-260">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="44999-260">Response 5</span></span>

<span data-ttu-id="44999-261">Here is the response from the fifth example which contains the new conversation and a thread ID.</span><span class="sxs-lookup"><span data-stu-id="44999-261">Here is the response from the fifth example which contains the new conversation and a thread ID.</span></span> <span data-ttu-id="44999-262">This new thread contains an automatically created post, which in turn contains the new extension.</span><span class="sxs-lookup"><span data-stu-id="44999-262">This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="44999-263">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="44999-263">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="44999-264">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="44999-264">All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="44999-265">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one.</span><span class="sxs-lookup"><span data-stu-id="44999-265">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one.</span></span> <span data-ttu-id="44999-266">Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="44999-266">Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

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
