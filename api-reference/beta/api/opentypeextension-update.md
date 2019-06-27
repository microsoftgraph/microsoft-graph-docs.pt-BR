---
title: Atualizar extensão aberta
description: 'Atualize uma extensão aberta (objeto openTypeExtension) com as propriedades no corpo da solicitação:'
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 0798c6fbf4d16742be863093cac1d98a8398cf0b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267834"
---
# <a name="update-open-extension"></a><span data-ttu-id="041db-103">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="041db-103">Update open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="041db-104">Atualize uma extensão aberta (objeto[openTypeExtension](../resources/opentypeextension.md) ) com as propriedades no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="041db-104">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="041db-105">Se uma propriedade no corpo da solicitação corresponder ao nome de uma propriedade existente na extensão, os dados na extensão serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="041db-105">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="041db-106">Caso contrário, essa propriedade e seus dados serão adicionados à extensão.</span><span class="sxs-lookup"><span data-stu-id="041db-106">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="041db-107">Os dados em uma extensão podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="041db-107">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="041db-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="041db-108">Permissions</span></span>

<span data-ttu-id="041db-109">Dependendo do recurso no qual a extensão foi criada e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="041db-109">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="041db-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="041db-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="041db-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="041db-111">Supported resource</span></span> | <span data-ttu-id="041db-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="041db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="041db-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="041db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="041db-114">Application</span><span class="sxs-lookup"><span data-stu-id="041db-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="041db-115">device</span><span class="sxs-lookup"><span data-stu-id="041db-115">device</span></span>](../resources/device.md) | <span data-ttu-id="041db-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="041db-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="041db-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="041db-117">Not supported</span></span> | <span data-ttu-id="041db-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="041db-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="041db-119">evento</span><span class="sxs-lookup"><span data-stu-id="041db-119">event</span></span>](../resources/event.md) | <span data-ttu-id="041db-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="041db-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="041db-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="041db-123">grupo</span><span class="sxs-lookup"><span data-stu-id="041db-123">group</span></span>](../resources/group.md) | <span data-ttu-id="041db-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="041db-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="041db-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="041db-125">Not supported</span></span> | <span data-ttu-id="041db-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="041db-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="041db-127">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="041db-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="041db-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="041db-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="041db-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="041db-129">Not supported</span></span> | <span data-ttu-id="041db-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="041db-130">Not supported</span></span> |
| [<span data-ttu-id="041db-131">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="041db-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="041db-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="041db-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="041db-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="041db-133">Not supported</span></span> | <span data-ttu-id="041db-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="041db-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="041db-135">mensagem</span><span class="sxs-lookup"><span data-stu-id="041db-135">message</span></span>](../resources/message.md) | <span data-ttu-id="041db-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-136">Mail.ReadWrite</span></span> | <span data-ttu-id="041db-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-137">Mail.ReadWrite</span></span> | <span data-ttu-id="041db-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="041db-139">organização</span><span class="sxs-lookup"><span data-stu-id="041db-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="041db-140">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="041db-140">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="041db-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="041db-141">Not supported</span></span> | <span data-ttu-id="041db-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="041db-142">Not supported</span></span> |
| [<span data-ttu-id="041db-143">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="041db-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="041db-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="041db-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="041db-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="041db-147">user</span><span class="sxs-lookup"><span data-stu-id="041db-147">user</span></span>](../resources/user.md) | <span data-ttu-id="041db-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="041db-148">User.ReadWrite.All</span></span> | <span data-ttu-id="041db-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041db-149">User.ReadWrite</span></span> | <span data-ttu-id="041db-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="041db-150">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="041db-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="041db-151">HTTP request</span></span>

<span data-ttu-id="041db-152">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `PATCH` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="041db-152">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

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

><span data-ttu-id="041db-153">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso, a fim de atualizar uma extensão nela.</span><span class="sxs-lookup"><span data-stu-id="041db-153">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it.</span></span> <span data-ttu-id="041db-154">Todas as outras sintaxes que permitem identificar essas instâncias de recurso oferecem suporte à atualização de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="041db-154">All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="041db-155">Confira a seção [Solicitar corpo](#request-body) sobre como incluir no corpo de solicitação dados personalizados para alterar ou adicionar a essa extensão.</span><span class="sxs-lookup"><span data-stu-id="041db-155">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="041db-156">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="041db-156">Path parameters</span></span>
|<span data-ttu-id="041db-157">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="041db-157">**Parameter**</span></span>|<span data-ttu-id="041db-158">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="041db-158">**Type**</span></span>|<span data-ttu-id="041db-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="041db-159">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="041db-160">id</span><span class="sxs-lookup"><span data-stu-id="041db-160">id</span></span>|<span data-ttu-id="041db-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="041db-161">string</span></span>|<span data-ttu-id="041db-p103">Um identificador exclusivo para uma instância da coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="041db-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="041db-164">extensionId</span><span class="sxs-lookup"><span data-stu-id="041db-164">extensionId</span></span>|<span data-ttu-id="041db-165">string</span><span class="sxs-lookup"><span data-stu-id="041db-165">string</span></span>|<span data-ttu-id="041db-p104">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="041db-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="041db-169">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="041db-169">Request headers</span></span>
| <span data-ttu-id="041db-170">Nome</span><span class="sxs-lookup"><span data-stu-id="041db-170">Name</span></span>       | <span data-ttu-id="041db-171">Valor</span><span class="sxs-lookup"><span data-stu-id="041db-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="041db-172">Autorização</span><span class="sxs-lookup"><span data-stu-id="041db-172">Authorization</span></span> | <span data-ttu-id="041db-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="041db-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="041db-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="041db-175">Content-Type</span></span> | <span data-ttu-id="041db-176">application/json</span><span class="sxs-lookup"><span data-stu-id="041db-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="041db-177">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="041db-177">Request body</span></span>

<span data-ttu-id="041db-p106">Forneça um corpo JSON de um objeto [openTypeExtension](../resources/opentypeextension.md), com os seguintes pares de nome e valor obrigatórios e os dados personalizados para alterar ou adicionar a essa extensão. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="041db-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="041db-180">Nome</span><span class="sxs-lookup"><span data-stu-id="041db-180">Name</span></span>       | <span data-ttu-id="041db-181">Valor</span><span class="sxs-lookup"><span data-stu-id="041db-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="041db-182">@odata.type</span><span class="sxs-lookup"><span data-stu-id="041db-182">@odata.type</span></span> | <span data-ttu-id="041db-183">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="041db-183">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="041db-184">extensionName</span><span class="sxs-lookup"><span data-stu-id="041db-184">extensionName</span></span> | <span data-ttu-id="041db-185">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="041db-185">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="041db-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="041db-186">Response</span></span>

<span data-ttu-id="041db-187">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [openTypeExtension](../resources/opentypeextension.md) atualizado.</span><span class="sxs-lookup"><span data-stu-id="041db-187">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="041db-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="041db-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="041db-189">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="041db-189">Request 1</span></span>

<span data-ttu-id="041db-p107">O primeiro exemplo mostra como atualizar uma extensão de uma mensagem. A extensão é representada inicialmente pela seguinte carga JSON:</span><span class="sxs-lookup"><span data-stu-id="041db-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

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

<span data-ttu-id="041db-192">Você pode fazer referência à extensão por seu nome:</span><span class="sxs-lookup"><span data-stu-id="041db-192">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="041db-193">Ou você pode fazer referência à extensão por seu nome totalmente qualificado:</span><span class="sxs-lookup"><span data-stu-id="041db-193">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="041db-194">Você pode usar o exemplo de solicitação e o seguinte corpo de solicitação para atualizar a extensão acima da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="041db-194">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="041db-195">Alterando `companyName` de `Wingtip Toys` para `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="041db-195">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="041db-196">Alterando `dealValue` de `500050` para `500100`</span><span class="sxs-lookup"><span data-stu-id="041db-196">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="041db-197">Adicionar novos dados como a propriedade personalizada `updated`</span><span class="sxs-lookup"><span data-stu-id="041db-197">Adding new data as the custom property `updated`</span></span>

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


#### <a name="response-1"></a><span data-ttu-id="041db-198">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="041db-198">Response 1</span></span>

<span data-ttu-id="041db-199">Aqui está a resposta que é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="041db-199">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="041db-200">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="041db-200">Request 2</span></span>

<span data-ttu-id="041db-p108">O segundo exemplo mostra como atualizar uma extensão em uma postagem de grupo. A extensão é representada inicialmente pela seguinte carga JSON, com um valor `expirationDate` de `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="041db-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

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

<span data-ttu-id="041db-203">A seguir estão a solicitação e o corpo da solicitação para alterar o `expirationDate` para `2016-07-30T11:00:00Z`:</span><span class="sxs-lookup"><span data-stu-id="041db-203">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

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

#### <a name="response-2"></a><span data-ttu-id="041db-204">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="041db-204">Response 2</span></span>

<span data-ttu-id="041db-205">Aqui está a resposta do segundo exemplo, que mostra o `expirationDate` atualizado na extensão.</span><span class="sxs-lookup"><span data-stu-id="041db-205">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="041db-206">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="041db-206">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="041db-207">C#</span><span class="sxs-lookup"><span data-stu-id="041db-207">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_opentypeextension-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="041db-208">Javascript</span><span class="sxs-lookup"><span data-stu-id="041db-208">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_opentypeextension-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="041db-209">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="041db-209">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_opentypeextension-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/opentypeextension-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/opentypeextension-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/opentypeextension-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
