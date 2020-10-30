---
title: Atualizar extensão aberta
description: 'Atualize uma extensão aberta (objeto openTypeExtension) com as propriedades no corpo da solicitação:'
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 033d85d599260f1e2320c8595aca0b21ff58a046
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796924"
---
# <a name="update-open-extension"></a><span data-ttu-id="3fad6-103">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="3fad6-103">Update open extension</span></span>

<span data-ttu-id="3fad6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fad6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fad6-105">Atualize uma extensão aberta (objeto[openTypeExtension](../resources/opentypeextension.md) ) com as propriedades no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="3fad6-105">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="3fad6-106">Se uma propriedade no corpo da solicitação corresponder ao nome de uma propriedade existente na extensão, os dados na extensão serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="3fad6-106">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="3fad6-107">Caso contrário, essa propriedade e seus dados serão adicionados à extensão.</span><span class="sxs-lookup"><span data-stu-id="3fad6-107">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="3fad6-108">Os dados em uma extensão podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="3fad6-108">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fad6-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3fad6-109">Permissions</span></span>

<span data-ttu-id="3fad6-110">Dependendo do recurso no qual a extensão foi criada e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3fad6-110">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="3fad6-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fad6-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fad6-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="3fad6-112">Supported resource</span></span> | <span data-ttu-id="3fad6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fad6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3fad6-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fad6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fad6-115">Application</span><span class="sxs-lookup"><span data-stu-id="3fad6-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="3fad6-116">device</span><span class="sxs-lookup"><span data-stu-id="3fad6-116">device</span></span>](../resources/device.md) | <span data-ttu-id="3fad6-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-117">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="3fad6-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3fad6-118">Not supported</span></span> | <span data-ttu-id="3fad6-119">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-119">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="3fad6-120">evento</span><span class="sxs-lookup"><span data-stu-id="3fad6-120">event</span></span>](../resources/event.md) | <span data-ttu-id="3fad6-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="3fad6-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="3fad6-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-123">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="3fad6-124">grupo</span><span class="sxs-lookup"><span data-stu-id="3fad6-124">group</span></span>](../resources/group.md) | <span data-ttu-id="3fad6-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="3fad6-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3fad6-126">Not supported</span></span> | <span data-ttu-id="3fad6-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-127">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="3fad6-128">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="3fad6-128">group event</span></span>](../resources/event.md) | <span data-ttu-id="3fad6-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="3fad6-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3fad6-130">Not supported</span></span> | <span data-ttu-id="3fad6-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3fad6-131">Not supported</span></span> |
| [<span data-ttu-id="3fad6-132">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="3fad6-132">group post</span></span>](../resources/post.md) | <span data-ttu-id="3fad6-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-133">Group.ReadWrite.All</span></span> | <span data-ttu-id="3fad6-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3fad6-134">Not supported</span></span> | <span data-ttu-id="3fad6-135">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-135">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="3fad6-136">mensagem</span><span class="sxs-lookup"><span data-stu-id="3fad6-136">message</span></span>](../resources/message.md) | <span data-ttu-id="3fad6-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-137">Mail.ReadWrite</span></span> | <span data-ttu-id="3fad6-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-138">Mail.ReadWrite</span></span> | <span data-ttu-id="3fad6-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-139">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="3fad6-140">organization</span><span class="sxs-lookup"><span data-stu-id="3fad6-140">organization</span></span>](../resources/organization.md) | <span data-ttu-id="3fad6-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-141">Organization.ReadWrite.All</span></span> | <span data-ttu-id="3fad6-142">Incompatível</span><span class="sxs-lookup"><span data-stu-id="3fad6-142">Not supported</span></span> | <span data-ttu-id="3fad6-143">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-143">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="3fad6-144">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="3fad6-144">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="3fad6-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="3fad6-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="3fad6-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-147">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="3fad6-148">user</span><span class="sxs-lookup"><span data-stu-id="3fad6-148">user</span></span>](../resources/user.md) | <span data-ttu-id="3fad6-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-149">User.ReadWrite</span></span> | <span data-ttu-id="3fad6-150">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-150">User.ReadWrite</span></span> | <span data-ttu-id="3fad6-151">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fad6-151">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="3fad6-152">task</span><span class="sxs-lookup"><span data-stu-id="3fad6-152">task</span></span>](../resources/todotask.md) | <span data-ttu-id="3fad6-153">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-153">Tasks.ReadWrite</span></span> | <span data-ttu-id="3fad6-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-154">Tasks.ReadWrite</span></span> | <span data-ttu-id="3fad6-155">Tasks. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3fad6-155">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="3fad6-156">TaskList</span><span class="sxs-lookup"><span data-stu-id="3fad6-156">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="3fad6-157">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-157">Tasks.ReadWrite</span></span> | <span data-ttu-id="3fad6-158">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fad6-158">Tasks.ReadWrite</span></span> | <span data-ttu-id="3fad6-159">Tasks. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3fad6-159">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fad6-160">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fad6-160">HTTP request</span></span>
<span data-ttu-id="3fad6-161">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `PATCH` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="3fad6-161">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

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
PATCH /users/me/todo/lists/{todoTaskListId}/tasks/{taskId}/extensions/{extensionId}
PATCH /users/me/todo/lists/{todoTaskListId}/extensions/{extensionId}
```

><span data-ttu-id="3fad6-162">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso, a fim de atualizar uma extensão nela.</span><span class="sxs-lookup"><span data-stu-id="3fad6-162">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it.</span></span> <span data-ttu-id="3fad6-163">Todas as outras sintaxes que permitem identificar essas instâncias de recurso oferecem suporte à atualização de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="3fad6-163">All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="3fad6-164">Confira a seção [Solicitar corpo](#request-body) sobre como incluir no corpo de solicitação dados personalizados para alterar ou adicionar a essa extensão.</span><span class="sxs-lookup"><span data-stu-id="3fad6-164">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="3fad6-165">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="3fad6-165">Path parameters</span></span>
|<span data-ttu-id="3fad6-166">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3fad6-166">Parameter</span></span>|<span data-ttu-id="3fad6-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fad6-167">Type</span></span>|<span data-ttu-id="3fad6-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fad6-168">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3fad6-169">id</span><span class="sxs-lookup"><span data-stu-id="3fad6-169">id</span></span>|<span data-ttu-id="3fad6-170">string</span><span class="sxs-lookup"><span data-stu-id="3fad6-170">string</span></span>|<span data-ttu-id="3fad6-p103">Um identificador exclusivo para uma instância da coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fad6-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="3fad6-173">extensionId</span><span class="sxs-lookup"><span data-stu-id="3fad6-173">extensionId</span></span>|<span data-ttu-id="3fad6-174">string</span><span class="sxs-lookup"><span data-stu-id="3fad6-174">string</span></span>|<span data-ttu-id="3fad6-p104">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fad6-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3fad6-178">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fad6-178">Request headers</span></span>
| <span data-ttu-id="3fad6-179">Nome</span><span class="sxs-lookup"><span data-stu-id="3fad6-179">Name</span></span>       | <span data-ttu-id="3fad6-180">Valor</span><span class="sxs-lookup"><span data-stu-id="3fad6-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3fad6-181">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fad6-181">Authorization</span></span> | <span data-ttu-id="3fad6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fad6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3fad6-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3fad6-184">Content-Type</span></span> | <span data-ttu-id="3fad6-185">application/json</span><span class="sxs-lookup"><span data-stu-id="3fad6-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fad6-186">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fad6-186">Request body</span></span>

<span data-ttu-id="3fad6-p106">Forneça um corpo JSON de um objeto [openTypeExtension](../resources/opentypeextension.md), com os seguintes pares de nome e valor obrigatórios e os dados personalizados para alterar ou adicionar a essa extensão. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="3fad6-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="3fad6-189">Nome</span><span class="sxs-lookup"><span data-stu-id="3fad6-189">Name</span></span>       | <span data-ttu-id="3fad6-190">Valor</span><span class="sxs-lookup"><span data-stu-id="3fad6-190">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3fad6-191">@odata.type</span><span class="sxs-lookup"><span data-stu-id="3fad6-191">@odata.type</span></span> | <span data-ttu-id="3fad6-192">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="3fad6-192">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="3fad6-193">extensionName</span><span class="sxs-lookup"><span data-stu-id="3fad6-193">extensionName</span></span> | <span data-ttu-id="3fad6-194">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="3fad6-194">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="3fad6-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fad6-195">Response</span></span>

<span data-ttu-id="3fad6-196">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [openTypeExtension](../resources/opentypeextension.md) atualizado.</span><span class="sxs-lookup"><span data-stu-id="3fad6-196">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="3fad6-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fad6-197">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="3fad6-198">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="3fad6-198">Request 1</span></span>

<span data-ttu-id="3fad6-p107">O primeiro exemplo mostra como atualizar uma extensão de uma mensagem. A extensão é representada inicialmente pela seguinte carga JSON:</span><span class="sxs-lookup"><span data-stu-id="3fad6-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

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

<span data-ttu-id="3fad6-201">Você pode fazer referência à extensão por seu nome:</span><span class="sxs-lookup"><span data-stu-id="3fad6-201">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="3fad6-202">Ou você pode fazer referência à extensão por seu nome totalmente qualificado:</span><span class="sxs-lookup"><span data-stu-id="3fad6-202">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="3fad6-203">Você pode usar o exemplo de solicitação e o seguinte corpo de solicitação para atualizar a extensão acima da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="3fad6-203">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="3fad6-204">Alterando `companyName` de `Wingtip Toys` para `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="3fad6-204">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="3fad6-205">Alterando `dealValue` de `500050` para `500100`</span><span class="sxs-lookup"><span data-stu-id="3fad6-205">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="3fad6-206">Adicionar novos dados como a propriedade personalizada `updated`</span><span class="sxs-lookup"><span data-stu-id="3fad6-206">Adding new data as the custom property `updated`</span></span>

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


#### <a name="response-1"></a><span data-ttu-id="3fad6-207">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="3fad6-207">Response 1</span></span>

<span data-ttu-id="3fad6-208">Aqui está a resposta que é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="3fad6-208">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="3fad6-209">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="3fad6-209">Request 2</span></span>

<span data-ttu-id="3fad6-p108">O segundo exemplo mostra como atualizar uma extensão em uma postagem de grupo. A extensão é representada inicialmente pela seguinte carga JSON, com um valor `expirationDate` de `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="3fad6-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

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

<span data-ttu-id="3fad6-212">A seguir estão a solicitação e o corpo da solicitação para alterar o `expirationDate` para `2016-07-30T11:00:00Z`:</span><span class="sxs-lookup"><span data-stu-id="3fad6-212">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

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

#### <a name="response-2"></a><span data-ttu-id="3fad6-213">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="3fad6-213">Response 2</span></span>

<span data-ttu-id="3fad6-214">Aqui está a resposta do segundo exemplo, que mostra o `expirationDate` atualizado na extensão.</span><span class="sxs-lookup"><span data-stu-id="3fad6-214">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

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

