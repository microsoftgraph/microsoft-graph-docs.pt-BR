---
title: Atualizar extensão aberta
description: 'Atualize uma extensão aberta (objeto openTypeExtension) com as propriedades no corpo da solicitação:'
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 1f9f75d4992e41abbeddfd52ca8054d837cb842f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414396"
---
# <a name="update-open-extension"></a><span data-ttu-id="1ee01-103">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="1ee01-103">Update open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ee01-104">Atualize uma extensão aberta (objeto[openTypeExtension](../resources/opentypeextension.md) ) com as propriedades no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="1ee01-104">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="1ee01-105">Se uma propriedade no corpo da solicitação corresponder ao nome de uma propriedade existente na extensão, os dados na extensão serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="1ee01-105">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="1ee01-106">Caso contrário, essa propriedade e seus dados serão adicionados à extensão.</span><span class="sxs-lookup"><span data-stu-id="1ee01-106">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="1ee01-107">Os dados em uma extensão podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="1ee01-107">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ee01-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ee01-108">Permissions</span></span>

<span data-ttu-id="1ee01-109">Dependendo do recurso no qual a extensão foi criada e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1ee01-109">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="1ee01-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ee01-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ee01-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="1ee01-111">Supported resource</span></span> | <span data-ttu-id="1ee01-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ee01-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1ee01-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ee01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ee01-114">Application</span><span class="sxs-lookup"><span data-stu-id="1ee01-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="1ee01-115">device</span><span class="sxs-lookup"><span data-stu-id="1ee01-115">device</span></span>](../resources/device.md) | <span data-ttu-id="1ee01-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="1ee01-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1ee01-117">Not supported</span></span> | <span data-ttu-id="1ee01-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="1ee01-119">evento</span><span class="sxs-lookup"><span data-stu-id="1ee01-119">event</span></span>](../resources/event.md) | <span data-ttu-id="1ee01-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="1ee01-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="1ee01-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="1ee01-123">grupo</span><span class="sxs-lookup"><span data-stu-id="1ee01-123">group</span></span>](../resources/group.md) | <span data-ttu-id="1ee01-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="1ee01-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1ee01-125">Not supported</span></span> | <span data-ttu-id="1ee01-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="1ee01-127">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="1ee01-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="1ee01-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="1ee01-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1ee01-129">Not supported</span></span> | <span data-ttu-id="1ee01-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1ee01-130">Not supported</span></span> |
| [<span data-ttu-id="1ee01-131">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="1ee01-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="1ee01-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="1ee01-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1ee01-133">Not supported</span></span> | <span data-ttu-id="1ee01-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="1ee01-135">mensagem</span><span class="sxs-lookup"><span data-stu-id="1ee01-135">message</span></span>](../resources/message.md) | <span data-ttu-id="1ee01-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-136">Mail.ReadWrite</span></span> | <span data-ttu-id="1ee01-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-137">Mail.ReadWrite</span></span> | <span data-ttu-id="1ee01-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="1ee01-139">organização</span><span class="sxs-lookup"><span data-stu-id="1ee01-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="1ee01-140">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-140">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="1ee01-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1ee01-141">Not supported</span></span> | <span data-ttu-id="1ee01-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1ee01-142">Not supported</span></span> |
| [<span data-ttu-id="1ee01-143">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="1ee01-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="1ee01-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="1ee01-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="1ee01-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="1ee01-147">user</span><span class="sxs-lookup"><span data-stu-id="1ee01-147">user</span></span>](../resources/user.md) | <span data-ttu-id="1ee01-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-148">User.ReadWrite.All</span></span> | <span data-ttu-id="1ee01-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee01-149">User.ReadWrite</span></span> | <span data-ttu-id="1ee01-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee01-150">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ee01-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ee01-151">HTTP request</span></span>

<span data-ttu-id="1ee01-152">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `PATCH` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="1ee01-152">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{Id}/extensions/{extensionId}
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

><span data-ttu-id="1ee01-153">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso, a fim de atualizar uma extensão nela.</span><span class="sxs-lookup"><span data-stu-id="1ee01-153">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it.</span></span> <span data-ttu-id="1ee01-154">Todas as outras sintaxes que permitem identificar essas instâncias de recurso oferecem suporte à atualização de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="1ee01-154">All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="1ee01-155">Confira a seção [Solicitar corpo](#request-body) sobre como incluir no corpo de solicitação dados personalizados para alterar ou adicionar a essa extensão.</span><span class="sxs-lookup"><span data-stu-id="1ee01-155">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="1ee01-156">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1ee01-156">Path parameters</span></span>
|<span data-ttu-id="1ee01-157">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="1ee01-157">**Parameter**</span></span>|<span data-ttu-id="1ee01-158">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="1ee01-158">**Type**</span></span>|<span data-ttu-id="1ee01-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1ee01-159">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1ee01-160">id</span><span class="sxs-lookup"><span data-stu-id="1ee01-160">id</span></span>|<span data-ttu-id="1ee01-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ee01-161">string</span></span>|<span data-ttu-id="1ee01-p103">Um identificador exclusivo para uma instância da coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ee01-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="1ee01-164">extensionId</span><span class="sxs-lookup"><span data-stu-id="1ee01-164">extensionId</span></span>|<span data-ttu-id="1ee01-165">string</span><span class="sxs-lookup"><span data-stu-id="1ee01-165">string</span></span>|<span data-ttu-id="1ee01-p104">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ee01-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1ee01-169">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ee01-169">Request headers</span></span>
| <span data-ttu-id="1ee01-170">Nome</span><span class="sxs-lookup"><span data-stu-id="1ee01-170">Name</span></span>       | <span data-ttu-id="1ee01-171">Valor</span><span class="sxs-lookup"><span data-stu-id="1ee01-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1ee01-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ee01-172">Authorization</span></span> | <span data-ttu-id="1ee01-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ee01-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ee01-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ee01-175">Content-Type</span></span> | <span data-ttu-id="1ee01-176">application/json</span><span class="sxs-lookup"><span data-stu-id="1ee01-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ee01-177">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ee01-177">Request body</span></span>

<span data-ttu-id="1ee01-p106">Forneça um corpo JSON de um objeto [openTypeExtension](../resources/opentypeextension.md), com os seguintes pares de nome e valor obrigatórios e os dados personalizados para alterar ou adicionar a essa extensão. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="1ee01-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="1ee01-180">Nome</span><span class="sxs-lookup"><span data-stu-id="1ee01-180">Name</span></span>       | <span data-ttu-id="1ee01-181">Valor</span><span class="sxs-lookup"><span data-stu-id="1ee01-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1ee01-182">@odata.type</span><span class="sxs-lookup"><span data-stu-id="1ee01-182">@odata.type</span></span> | <span data-ttu-id="1ee01-183">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="1ee01-183">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="1ee01-184">extensionName</span><span class="sxs-lookup"><span data-stu-id="1ee01-184">extensionName</span></span> | <span data-ttu-id="1ee01-185">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="1ee01-185">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="1ee01-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ee01-186">Response</span></span>

<span data-ttu-id="1ee01-187">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [openTypeExtension](../resources/opentypeextension.md) atualizado.</span><span class="sxs-lookup"><span data-stu-id="1ee01-187">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="1ee01-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ee01-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="1ee01-189">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="1ee01-189">Request 1</span></span>

<span data-ttu-id="1ee01-p107">O primeiro exemplo mostra como atualizar uma extensão de uma mensagem. A extensão é representada inicialmente pela seguinte carga JSON:</span><span class="sxs-lookup"><span data-stu-id="1ee01-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="1ee01-192">Você pode fazer referência à extensão por seu nome:</span><span class="sxs-lookup"><span data-stu-id="1ee01-192">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="1ee01-193">Ou você pode fazer referência à extensão por seu nome totalmente qualificado:</span><span class="sxs-lookup"><span data-stu-id="1ee01-193">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="1ee01-194">Você pode usar o exemplo de solicitação e o seguinte corpo de solicitação para atualizar a extensão acima da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="1ee01-194">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="1ee01-195">Alterando `companyName` de `Wingtip Toys` para `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="1ee01-195">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="1ee01-196">Alterando `dealValue` de `500050` para `500100`</span><span class="sxs-lookup"><span data-stu-id="1ee01-196">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="1ee01-197">Adicionar novos dados como a propriedade personalizada `updated`</span><span class="sxs-lookup"><span data-stu-id="1ee01-197">Adding new data as the custom property `updated`</span></span>

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


#### <a name="response-1"></a><span data-ttu-id="1ee01-198">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="1ee01-198">Response 1</span></span>

<span data-ttu-id="1ee01-199">Aqui está a resposta que é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="1ee01-199">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
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

#### <a name="request-2"></a><span data-ttu-id="1ee01-200">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="1ee01-200">Request 2</span></span>

<span data-ttu-id="1ee01-p108">O segundo exemplo mostra como atualizar uma extensão em uma postagem de grupo. A extensão é representada inicialmente pela seguinte carga JSON, com um valor `expirationDate` de `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="1ee01-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
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

<span data-ttu-id="1ee01-203">A seguir estão a solicitação e o corpo da solicitação para alterar o `expirationDate` para `2016-07-30T11:00:00Z`:</span><span class="sxs-lookup"><span data-stu-id="1ee01-203">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1ee01-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ee01-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
Content-type: application/json

{
   "@odata.type": "#microsoft.outlookServices.openTypeExtension",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ee01-205">C#</span><span class="sxs-lookup"><span data-stu-id="1ee01-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ee01-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ee01-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1ee01-207">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1ee01-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="1ee01-208">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="1ee01-208">Response 2</span></span>

<span data-ttu-id="1ee01-209">Aqui está a resposta do segundo exemplo, que mostra o `expirationDate` atualizado na extensão.</span><span class="sxs-lookup"><span data-stu-id="1ee01-209">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "response",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.openTypeExtension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
