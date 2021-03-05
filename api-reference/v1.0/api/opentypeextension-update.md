---
title: Atualizar extensão aberta
description: 'Atualize uma extensão aberta (objeto openTypeExtension) com as propriedades no corpo da solicitação:'
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: e32fc9a5a37453bfe77a2fa4a8539d69ebedef6f
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470708"
---
# <a name="update-open-extension"></a><span data-ttu-id="8f4ae-103">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="8f4ae-103">Update open extension</span></span>

<span data-ttu-id="8f4ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f4ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f4ae-105">Atualize uma extensão aberta[(objeto openTypeExtension)](../resources/opentypeextension.md) com as propriedades no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="8f4ae-105">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="8f4ae-106">Se uma propriedade no corpo da solicitação corresponder ao nome de uma propriedade existente na extensão, os dados na extensão serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-106">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="8f4ae-107">Caso contrário, essa propriedade e seus dados serão adicionados à extensão.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-107">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="8f4ae-108">Os dados em uma extensão podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-108">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

<span data-ttu-id="8f4ae-109">Consulte a tabela na seção [Permissões](#permissions) para a lista de recursos que suportam extensões abertas.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-109">See the table in the [Permissions](#permissions) section for the list of resources that support open extensions.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f4ae-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f4ae-110">Permissions</span></span>

<span data-ttu-id="8f4ae-111">Dependendo do recurso no qual a extensão foi criada e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo privilegiado necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-111">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8f4ae-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f4ae-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f4ae-113">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="8f4ae-113">Supported resource</span></span> | <span data-ttu-id="8f4ae-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f4ae-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8f4ae-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f4ae-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f4ae-116">Application</span><span class="sxs-lookup"><span data-stu-id="8f4ae-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="8f4ae-117">device</span><span class="sxs-lookup"><span data-stu-id="8f4ae-117">device</span></span>](../resources/device.md) | <span data-ttu-id="8f4ae-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-118">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="8f4ae-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8f4ae-119">Not supported</span></span> | <span data-ttu-id="8f4ae-120">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-120">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="8f4ae-121">evento</span><span class="sxs-lookup"><span data-stu-id="8f4ae-121">event</span></span>](../resources/event.md) | <span data-ttu-id="8f4ae-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="8f4ae-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="8f4ae-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-124">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="8f4ae-125">grupo</span><span class="sxs-lookup"><span data-stu-id="8f4ae-125">group</span></span>](../resources/group.md) | <span data-ttu-id="8f4ae-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="8f4ae-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8f4ae-127">Not supported</span></span> | <span data-ttu-id="8f4ae-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-128">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="8f4ae-129">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="8f4ae-129">group event</span></span>](../resources/event.md) | <span data-ttu-id="8f4ae-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="8f4ae-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8f4ae-131">Not supported</span></span> | <span data-ttu-id="8f4ae-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8f4ae-132">Not supported</span></span> |
| [<span data-ttu-id="8f4ae-133">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="8f4ae-133">group post</span></span>](../resources/post.md) | <span data-ttu-id="8f4ae-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-134">Group.ReadWrite.All</span></span> | <span data-ttu-id="8f4ae-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8f4ae-135">Not supported</span></span> | <span data-ttu-id="8f4ae-136">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-136">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="8f4ae-137">mensagem</span><span class="sxs-lookup"><span data-stu-id="8f4ae-137">message</span></span>](../resources/message.md) | <span data-ttu-id="8f4ae-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-138">Mail.ReadWrite</span></span> | <span data-ttu-id="8f4ae-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-139">Mail.ReadWrite</span></span> | <span data-ttu-id="8f4ae-140">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-140">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="8f4ae-141">organization</span><span class="sxs-lookup"><span data-stu-id="8f4ae-141">organization</span></span>](../resources/organization.md) | <span data-ttu-id="8f4ae-142">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-142">Organization.ReadWrite.All</span></span> | <span data-ttu-id="8f4ae-143">Incompatível</span><span class="sxs-lookup"><span data-stu-id="8f4ae-143">Not supported</span></span> | <span data-ttu-id="8f4ae-144">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-144">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="8f4ae-145">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="8f4ae-145">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="8f4ae-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="8f4ae-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-147">Contacts.ReadWrite</span></span> | <span data-ttu-id="8f4ae-148">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-148">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="8f4ae-149">user</span><span class="sxs-lookup"><span data-stu-id="8f4ae-149">user</span></span>](../resources/user.md) | <span data-ttu-id="8f4ae-150">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-150">User.ReadWrite</span></span> | <span data-ttu-id="8f4ae-151">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-151">User.ReadWrite</span></span> | <span data-ttu-id="8f4ae-152">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-152">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="8f4ae-153">tarefa</span><span class="sxs-lookup"><span data-stu-id="8f4ae-153">task</span></span>](../resources/todotask.md) | <span data-ttu-id="8f4ae-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-154">Tasks.ReadWrite</span></span> | <span data-ttu-id="8f4ae-155">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-155">Tasks.ReadWrite</span></span> | <span data-ttu-id="8f4ae-156">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-156">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="8f4ae-157">tasklist</span><span class="sxs-lookup"><span data-stu-id="8f4ae-157">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="8f4ae-158">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-158">Tasks.ReadWrite</span></span> | <span data-ttu-id="8f4ae-159">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ae-159">Tasks.ReadWrite</span></span> | <span data-ttu-id="8f4ae-160">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4ae-160">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f4ae-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f4ae-161">HTTP request</span></span>
<span data-ttu-id="8f4ae-162">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `PATCH` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-162">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

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

><span data-ttu-id="8f4ae-163">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso, a fim de atualizar uma extensão nele.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-163">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it.</span></span> <span data-ttu-id="8f4ae-164">Todas as outras sintaxes que permitem identificar essas instâncias de recursos suportam a atualização de extensões abertas neles de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-164">All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="8f4ae-165">Confira a seção [Solicitar corpo](#request-body) sobre como incluir no corpo de solicitação dados personalizados para alterar ou adicionar a essa extensão.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-165">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="8f4ae-166">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="8f4ae-166">Path parameters</span></span>
|<span data-ttu-id="8f4ae-167">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8f4ae-167">Parameter</span></span>|<span data-ttu-id="8f4ae-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f4ae-168">Type</span></span>|<span data-ttu-id="8f4ae-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f4ae-169">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8f4ae-170">id</span><span class="sxs-lookup"><span data-stu-id="8f4ae-170">id</span></span>|<span data-ttu-id="8f4ae-171">string</span><span class="sxs-lookup"><span data-stu-id="8f4ae-171">string</span></span>|<span data-ttu-id="8f4ae-p103">Um identificador exclusivo para uma instância da coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="8f4ae-174">extensionId</span><span class="sxs-lookup"><span data-stu-id="8f4ae-174">extensionId</span></span>|<span data-ttu-id="8f4ae-175">string</span><span class="sxs-lookup"><span data-stu-id="8f4ae-175">string</span></span>|<span data-ttu-id="8f4ae-p104">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8f4ae-179">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f4ae-179">Request headers</span></span>
| <span data-ttu-id="8f4ae-180">Nome</span><span class="sxs-lookup"><span data-stu-id="8f4ae-180">Name</span></span>       | <span data-ttu-id="8f4ae-181">Valor</span><span class="sxs-lookup"><span data-stu-id="8f4ae-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="8f4ae-182">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f4ae-182">Authorization</span></span> | <span data-ttu-id="8f4ae-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f4ae-185">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f4ae-185">Content-Type</span></span> | <span data-ttu-id="8f4ae-186">application/json</span><span class="sxs-lookup"><span data-stu-id="8f4ae-186">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f4ae-187">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f4ae-187">Request body</span></span>

<span data-ttu-id="8f4ae-p106">Forneça um corpo JSON de um objeto [openTypeExtension](../resources/opentypeextension.md), com os seguintes pares de nome e valor obrigatórios e os dados personalizados para alterar ou adicionar a essa extensão. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="8f4ae-190">Nome</span><span class="sxs-lookup"><span data-stu-id="8f4ae-190">Name</span></span>       | <span data-ttu-id="8f4ae-191">Valor</span><span class="sxs-lookup"><span data-stu-id="8f4ae-191">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="8f4ae-192">@odata.type</span><span class="sxs-lookup"><span data-stu-id="8f4ae-192">@odata.type</span></span> | <span data-ttu-id="8f4ae-193">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="8f4ae-193">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="8f4ae-194">extensionName</span><span class="sxs-lookup"><span data-stu-id="8f4ae-194">extensionName</span></span> | <span data-ttu-id="8f4ae-195">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="8f4ae-195">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="8f4ae-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f4ae-196">Response</span></span>

<span data-ttu-id="8f4ae-197">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [openTypeExtension](../resources/opentypeextension.md) atualizado.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-197">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="8f4ae-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f4ae-198">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="8f4ae-199">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="8f4ae-199">Request 1</span></span>

<span data-ttu-id="8f4ae-p107">O primeiro exemplo mostra como atualizar uma extensão de uma mensagem. A extensão é representada inicialmente pela seguinte carga JSON:</span><span class="sxs-lookup"><span data-stu-id="8f4ae-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

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

<span data-ttu-id="8f4ae-202">Você pode fazer referência à extensão por seu nome:</span><span class="sxs-lookup"><span data-stu-id="8f4ae-202">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="8f4ae-203">Ou você pode fazer referência à extensão por seu nome totalmente qualificado:</span><span class="sxs-lookup"><span data-stu-id="8f4ae-203">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="8f4ae-204">Você pode usar o exemplo de solicitação e o seguinte corpo de solicitação para atualizar a extensão acima da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="8f4ae-204">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="8f4ae-205">Alterando `companyName` de `Wingtip Toys` para `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="8f4ae-205">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="8f4ae-206">Alterando `dealValue` de `500050` para `500100`</span><span class="sxs-lookup"><span data-stu-id="8f4ae-206">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="8f4ae-207">Adicionar novos dados como a propriedade personalizada `updated`</span><span class="sxs-lookup"><span data-stu-id="8f4ae-207">Adding new data as the custom property `updated`</span></span>

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


#### <a name="response-1"></a><span data-ttu-id="8f4ae-208">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="8f4ae-208">Response 1</span></span>

<span data-ttu-id="8f4ae-209">Aqui está a resposta que é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-209">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="8f4ae-210">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="8f4ae-210">Request 2</span></span>

<span data-ttu-id="8f4ae-p108">O segundo exemplo mostra como atualizar uma extensão em uma postagem de grupo. A extensão é representada inicialmente pela seguinte carga JSON, com um valor `expirationDate` de `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="8f4ae-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

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

<span data-ttu-id="8f4ae-213">A seguir estão a solicitação e o corpo da solicitação para alterar o `expirationDate` para `2016-07-30T11:00:00Z`:</span><span class="sxs-lookup"><span data-stu-id="8f4ae-213">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>


# <a name="http"></a>[<span data-ttu-id="8f4ae-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f4ae-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="8f4ae-215">C#</span><span class="sxs-lookup"><span data-stu-id="8f4ae-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f4ae-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f4ae-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f4ae-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f4ae-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="8f4ae-218">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="8f4ae-218">Response 2</span></span>

<span data-ttu-id="8f4ae-219">Aqui está a resposta do segundo exemplo, que mostra o `expirationDate` atualizado na extensão.</span><span class="sxs-lookup"><span data-stu-id="8f4ae-219">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "response",  
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

