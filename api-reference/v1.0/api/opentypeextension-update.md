---
title: Atualizar extensão aberta
description: 'Atualize uma extensão aberta (objeto openTypeExtension) com as propriedades no corpo da solicitação:'
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 89804b1259f3832b2b69e2f62d25ac1fa8856809
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863688"
---
# <a name="update-open-extension"></a><span data-ttu-id="612d0-103">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="612d0-103">Update open extension</span></span>

<span data-ttu-id="612d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="612d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="612d0-105">Atualize uma extensão aberta (objeto[openTypeExtension](../resources/opentypeextension.md) ) com as propriedades no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="612d0-105">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="612d0-106">Se uma propriedade no corpo da solicitação corresponder ao nome de uma propriedade existente na extensão, os dados na extensão serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="612d0-106">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="612d0-107">Caso contrário, essa propriedade e seus dados serão adicionados à extensão.</span><span class="sxs-lookup"><span data-stu-id="612d0-107">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="612d0-108">Os dados em uma extensão podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="612d0-108">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="612d0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="612d0-109">Permissions</span></span>

<span data-ttu-id="612d0-110">Dependendo do recurso no qual a extensão foi criada e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="612d0-110">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="612d0-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="612d0-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="612d0-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="612d0-112">Supported resource</span></span> | <span data-ttu-id="612d0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="612d0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="612d0-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="612d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="612d0-115">Application</span><span class="sxs-lookup"><span data-stu-id="612d0-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="612d0-116">device</span><span class="sxs-lookup"><span data-stu-id="612d0-116">device</span></span>](../resources/device.md) | <span data-ttu-id="612d0-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="612d0-117">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="612d0-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="612d0-118">Not supported</span></span> | <span data-ttu-id="612d0-119">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-119">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="612d0-120">evento</span><span class="sxs-lookup"><span data-stu-id="612d0-120">event</span></span>](../resources/event.md) | <span data-ttu-id="612d0-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="612d0-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="612d0-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-123">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="612d0-124">grupo</span><span class="sxs-lookup"><span data-stu-id="612d0-124">group</span></span>](../resources/group.md) | <span data-ttu-id="612d0-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="612d0-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="612d0-126">Not supported</span></span> | <span data-ttu-id="612d0-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-127">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="612d0-128">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="612d0-128">group event</span></span>](../resources/event.md) | <span data-ttu-id="612d0-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="612d0-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="612d0-130">Not supported</span></span> | <span data-ttu-id="612d0-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="612d0-131">Not supported</span></span> |
| [<span data-ttu-id="612d0-132">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="612d0-132">group post</span></span>](../resources/post.md) | <span data-ttu-id="612d0-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-133">Group.ReadWrite.All</span></span> | <span data-ttu-id="612d0-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="612d0-134">Not supported</span></span> | <span data-ttu-id="612d0-135">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-135">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="612d0-136">mensagem</span><span class="sxs-lookup"><span data-stu-id="612d0-136">message</span></span>](../resources/message.md) | <span data-ttu-id="612d0-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-137">Mail.ReadWrite</span></span> | <span data-ttu-id="612d0-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-138">Mail.ReadWrite</span></span> | <span data-ttu-id="612d0-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-139">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="612d0-140">organização</span><span class="sxs-lookup"><span data-stu-id="612d0-140">organization</span></span>](../resources/organization.md) | <span data-ttu-id="612d0-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-141">Organization.ReadWrite.All</span></span> | <span data-ttu-id="612d0-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="612d0-142">Not supported</span></span> | <span data-ttu-id="612d0-143">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-143">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="612d0-144">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="612d0-144">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="612d0-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="612d0-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="612d0-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-147">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="612d0-148">user</span><span class="sxs-lookup"><span data-stu-id="612d0-148">user</span></span>](../resources/user.md) | <span data-ttu-id="612d0-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-149">User.ReadWrite</span></span> | <span data-ttu-id="612d0-150">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="612d0-150">User.ReadWrite</span></span> | <span data-ttu-id="612d0-151">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="612d0-151">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="612d0-152">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="612d0-152">HTTP request</span></span>
<span data-ttu-id="612d0-153">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `PATCH` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="612d0-153">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="612d0-154">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso, a fim de atualizar uma extensão nela.</span><span class="sxs-lookup"><span data-stu-id="612d0-154">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it.</span></span> <span data-ttu-id="612d0-155">Todas as outras sintaxes que permitem identificar essas instâncias de recurso oferecem suporte à atualização de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="612d0-155">All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="612d0-156">Confira a seção [Solicitar corpo](#request-body) sobre como incluir no corpo de solicitação dados personalizados para alterar ou adicionar a essa extensão.</span><span class="sxs-lookup"><span data-stu-id="612d0-156">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="612d0-157">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="612d0-157">Path parameters</span></span>
|<span data-ttu-id="612d0-158">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="612d0-158">Parameter</span></span>|<span data-ttu-id="612d0-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="612d0-159">Type</span></span>|<span data-ttu-id="612d0-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="612d0-160">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="612d0-161">id</span><span class="sxs-lookup"><span data-stu-id="612d0-161">id</span></span>|<span data-ttu-id="612d0-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="612d0-162">string</span></span>|<span data-ttu-id="612d0-163">A unique identifier for an instance of the corresponding collection.</span><span class="sxs-lookup"><span data-stu-id="612d0-163">A unique identifier for an instance of the corresponding collection.</span></span> <span data-ttu-id="612d0-164">Required.</span><span class="sxs-lookup"><span data-stu-id="612d0-164">Required.</span></span>|
|<span data-ttu-id="612d0-165">extensionId</span><span class="sxs-lookup"><span data-stu-id="612d0-165">extensionId</span></span>|<span data-ttu-id="612d0-166">string</span><span class="sxs-lookup"><span data-stu-id="612d0-166">string</span></span>|<span data-ttu-id="612d0-167">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier.</span><span class="sxs-lookup"><span data-stu-id="612d0-167">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier.</span></span> <span data-ttu-id="612d0-168">The fully qualified name is returned in the `id` property when you create the extension.</span><span class="sxs-lookup"><span data-stu-id="612d0-168">The fully qualified name is returned in the `id` property when you create the extension.</span></span> <span data-ttu-id="612d0-169">Required.</span><span class="sxs-lookup"><span data-stu-id="612d0-169">Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="612d0-170">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="612d0-170">Request headers</span></span>
| <span data-ttu-id="612d0-171">Nome</span><span class="sxs-lookup"><span data-stu-id="612d0-171">Name</span></span>       | <span data-ttu-id="612d0-172">Valor</span><span class="sxs-lookup"><span data-stu-id="612d0-172">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="612d0-173">Autorização</span><span class="sxs-lookup"><span data-stu-id="612d0-173">Authorization</span></span> | <span data-ttu-id="612d0-174">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="612d0-174">Bearer {token}.</span></span> <span data-ttu-id="612d0-175">Required.</span><span class="sxs-lookup"><span data-stu-id="612d0-175">Required.</span></span> |
| <span data-ttu-id="612d0-176">Content-Type</span><span class="sxs-lookup"><span data-stu-id="612d0-176">Content-Type</span></span> | <span data-ttu-id="612d0-177">application/json</span><span class="sxs-lookup"><span data-stu-id="612d0-177">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="612d0-178">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="612d0-178">Request body</span></span>

<span data-ttu-id="612d0-179">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension.</span><span class="sxs-lookup"><span data-stu-id="612d0-179">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension.</span></span> <span data-ttu-id="612d0-180">The data in the JSON payload can be primitive types, or arrays of primitive types.</span><span class="sxs-lookup"><span data-stu-id="612d0-180">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="612d0-181">Nome</span><span class="sxs-lookup"><span data-stu-id="612d0-181">Name</span></span>       | <span data-ttu-id="612d0-182">Valor</span><span class="sxs-lookup"><span data-stu-id="612d0-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="612d0-183">@odata.type</span><span class="sxs-lookup"><span data-stu-id="612d0-183">@odata.type</span></span> | <span data-ttu-id="612d0-184">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="612d0-184">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="612d0-185">extensionName</span><span class="sxs-lookup"><span data-stu-id="612d0-185">extensionName</span></span> | <span data-ttu-id="612d0-186">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="612d0-186">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="612d0-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="612d0-187">Response</span></span>

<span data-ttu-id="612d0-188">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [openTypeExtension](../resources/opentypeextension.md) atualizado.</span><span class="sxs-lookup"><span data-stu-id="612d0-188">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="612d0-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="612d0-189">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="612d0-190">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="612d0-190">Request 1</span></span>

<span data-ttu-id="612d0-191">The first example shows how to update an extension in a message.</span><span class="sxs-lookup"><span data-stu-id="612d0-191">The first example shows how to update an extension in a message.</span></span> <span data-ttu-id="612d0-192">The extension is initially represented by the following JSON payload:</span><span class="sxs-lookup"><span data-stu-id="612d0-192">The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="612d0-193">Você pode fazer referência à extensão por seu nome:</span><span class="sxs-lookup"><span data-stu-id="612d0-193">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="612d0-194">Ou você pode fazer referência à extensão por seu nome totalmente qualificado:</span><span class="sxs-lookup"><span data-stu-id="612d0-194">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="612d0-195">Você pode usar o exemplo de solicitação e o seguinte corpo de solicitação para atualizar a extensão acima da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="612d0-195">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="612d0-196">Alterando `companyName` de `Wingtip Toys` para `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="612d0-196">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="612d0-197">Alterando `dealValue` de `500050` para `500100`</span><span class="sxs-lookup"><span data-stu-id="612d0-197">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="612d0-198">Adicionar novos dados como a propriedade personalizada `updated`</span><span class="sxs-lookup"><span data-stu-id="612d0-198">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="612d0-199">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="612d0-199">Response 1</span></span>

<span data-ttu-id="612d0-200">Aqui está a resposta que é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="612d0-200">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="612d0-201">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="612d0-201">Request 2</span></span>

<span data-ttu-id="612d0-202">The second example shows how to update an extension in a group post.</span><span class="sxs-lookup"><span data-stu-id="612d0-202">The second example shows how to update an extension in a group post.</span></span> <span data-ttu-id="612d0-203">The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="612d0-203">The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="612d0-204">A seguir estão a solicitação e o corpo da solicitação para alterar o `expirationDate` para `2016-07-30T11:00:00Z`:</span><span class="sxs-lookup"><span data-stu-id="612d0-204">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"],
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="612d0-205">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="612d0-205">Response 2</span></span>

<span data-ttu-id="612d0-206">Aqui está a resposta do segundo exemplo, que mostra o `expirationDate` atualizado na extensão.</span><span class="sxs-lookup"><span data-stu-id="612d0-206">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "ignored",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.openTypeExtension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
