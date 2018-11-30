---
title: Atualizar extensão aberta
description: 'Atualize uma extensão aberta (objeto openTypeExtension) com as propriedades no corpo da solicitação:'
ms.openlocfilehash: 3b35ac56898aa910f0da5e3ac311fefd67fff12d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035043"
---
# <a name="update-open-extension"></a><span data-ttu-id="d3af2-103">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="d3af2-103">Update open extension</span></span>

> <span data-ttu-id="d3af2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3af2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3af2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3af2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3af2-106">Atualize uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) com as propriedades no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="d3af2-106">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="d3af2-107">Se uma propriedade no corpo da solicitação corresponder ao nome de uma propriedade existente na extensão, os dados na extensão serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="d3af2-107">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="d3af2-108">Caso contrário, essa propriedade e seus dados serão adicionados à extensão.</span><span class="sxs-lookup"><span data-stu-id="d3af2-108">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="d3af2-109">Os dados em uma extensão podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="d3af2-109">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3af2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3af2-110">Permissions</span></span>

<span data-ttu-id="d3af2-111">Dependendo do recurso que a extensão foi criada em e a permissão tipo (delegado ou aplicativo) solicitada, a permissão especificada na tabela a seguir é o menos privilegiada necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d3af2-111">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d3af2-112">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3af2-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3af2-113">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="d3af2-113">Supported resource</span></span> | <span data-ttu-id="d3af2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3af2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d3af2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3af2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3af2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3af2-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="d3af2-117">device</span><span class="sxs-lookup"><span data-stu-id="d3af2-117">device</span></span>](../resources/device.md) | <span data-ttu-id="d3af2-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-118">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="d3af2-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d3af2-119">Not supported</span></span> | <span data-ttu-id="d3af2-120">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-120">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="d3af2-121">evento</span><span class="sxs-lookup"><span data-stu-id="d3af2-121">event</span></span>](../resources/event.md) | <span data-ttu-id="d3af2-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="d3af2-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="d3af2-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-124">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="d3af2-125">grupo</span><span class="sxs-lookup"><span data-stu-id="d3af2-125">group</span></span>](../resources/group.md) | <span data-ttu-id="d3af2-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="d3af2-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d3af2-127">Not supported</span></span> | <span data-ttu-id="d3af2-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-128">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="d3af2-129">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="d3af2-129">group event</span></span>](../resources/event.md) | <span data-ttu-id="d3af2-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="d3af2-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d3af2-131">Not supported</span></span> | <span data-ttu-id="d3af2-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d3af2-132">Not supported</span></span> |
| [<span data-ttu-id="d3af2-133">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="d3af2-133">group post</span></span>](../resources/post.md) | <span data-ttu-id="d3af2-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-134">Group.ReadWrite.All</span></span> | <span data-ttu-id="d3af2-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d3af2-135">Not supported</span></span> | <span data-ttu-id="d3af2-136">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-136">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="d3af2-137">mensagem</span><span class="sxs-lookup"><span data-stu-id="d3af2-137">message</span></span>](../resources/message.md) | <span data-ttu-id="d3af2-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-138">Mail.ReadWrite</span></span> | <span data-ttu-id="d3af2-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-139">Mail.ReadWrite</span></span> | <span data-ttu-id="d3af2-140">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-140">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="d3af2-141">organização</span><span class="sxs-lookup"><span data-stu-id="d3af2-141">organization</span></span>](../resources/organization.md) | <span data-ttu-id="d3af2-142">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-142">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="d3af2-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d3af2-143">Not supported</span></span> | <span data-ttu-id="d3af2-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d3af2-144">Not supported</span></span> |
| [<span data-ttu-id="d3af2-145">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="d3af2-145">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="d3af2-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="d3af2-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-147">Contacts.ReadWrite</span></span> | <span data-ttu-id="d3af2-148">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-148">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="d3af2-149">usuário</span><span class="sxs-lookup"><span data-stu-id="d3af2-149">user</span></span>](../resources/user.md) | <span data-ttu-id="d3af2-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-150">User.ReadWrite.All</span></span> | <span data-ttu-id="d3af2-151">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3af2-151">User.ReadWrite</span></span> | <span data-ttu-id="d3af2-152">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3af2-152">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3af2-153">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3af2-153">HTTP request</span></span>

<span data-ttu-id="d3af2-154">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `PATCH` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="d3af2-154">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

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

><span data-ttu-id="d3af2-p103">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância do recurso, para atualizar uma extensão nele. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à atualização de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="d3af2-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="d3af2-157">Confira a seção [Solicitar corpo](#request-body) sobre como incluir no corpo de solicitação dados personalizados para alterar ou adicionar a essa extensão.</span><span class="sxs-lookup"><span data-stu-id="d3af2-157">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="d3af2-158">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d3af2-158">Path parameters</span></span>
|<span data-ttu-id="d3af2-159">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="d3af2-159">**Parameter**</span></span>|<span data-ttu-id="d3af2-160">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="d3af2-160">**Type**</span></span>|<span data-ttu-id="d3af2-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d3af2-161">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d3af2-162">id</span><span class="sxs-lookup"><span data-stu-id="d3af2-162">id</span></span>|<span data-ttu-id="d3af2-163">string</span><span class="sxs-lookup"><span data-stu-id="d3af2-163">string</span></span>|<span data-ttu-id="d3af2-p104">Um identificador exclusivo para uma instância da coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3af2-p104">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="d3af2-166">extensionId</span><span class="sxs-lookup"><span data-stu-id="d3af2-166">extensionId</span></span>|<span data-ttu-id="d3af2-167">string</span><span class="sxs-lookup"><span data-stu-id="d3af2-167">string</span></span>|<span data-ttu-id="d3af2-p105">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3af2-p105">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d3af2-171">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3af2-171">Request headers</span></span>
| <span data-ttu-id="d3af2-172">Nome</span><span class="sxs-lookup"><span data-stu-id="d3af2-172">Name</span></span>       | <span data-ttu-id="d3af2-173">Valor</span><span class="sxs-lookup"><span data-stu-id="d3af2-173">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d3af2-174">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3af2-174">Authorization</span></span> | <span data-ttu-id="d3af2-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3af2-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3af2-177">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3af2-177">Content-Type</span></span> | <span data-ttu-id="d3af2-178">application/json</span><span class="sxs-lookup"><span data-stu-id="d3af2-178">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3af2-179">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3af2-179">Request body</span></span>

<span data-ttu-id="d3af2-p107">Forneça um corpo JSON de um objeto [openTypeExtension](../resources/opentypeextension.md), com os seguintes pares de nome e valor obrigatórios e os dados personalizados para alterar ou adicionar a essa extensão. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="d3af2-p107">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="d3af2-182">Nome</span><span class="sxs-lookup"><span data-stu-id="d3af2-182">Name</span></span>       | <span data-ttu-id="d3af2-183">Valor</span><span class="sxs-lookup"><span data-stu-id="d3af2-183">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d3af2-184">@odata.type</span><span class="sxs-lookup"><span data-stu-id="d3af2-184">@odata.type</span></span> | <span data-ttu-id="d3af2-185">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="d3af2-185">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="d3af2-186">extensionName</span><span class="sxs-lookup"><span data-stu-id="d3af2-186">extensionName</span></span> | <span data-ttu-id="d3af2-187">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="d3af2-187">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="d3af2-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3af2-188">Response</span></span>

<span data-ttu-id="d3af2-189">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [openTypeExtension](../resources/opentypeextension.md) atualizado.</span><span class="sxs-lookup"><span data-stu-id="d3af2-189">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="d3af2-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3af2-190">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="d3af2-191">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="d3af2-191">Request 1</span></span>

<span data-ttu-id="d3af2-p108">O primeiro exemplo mostra como atualizar uma extensão de uma mensagem. A extensão é representada inicialmente pela seguinte carga JSON:</span><span class="sxs-lookup"><span data-stu-id="d3af2-p108">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="d3af2-194">Você pode fazer referência à extensão por seu nome:</span><span class="sxs-lookup"><span data-stu-id="d3af2-194">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="d3af2-195">Ou você pode fazer referência à extensão por seu nome totalmente qualificado:</span><span class="sxs-lookup"><span data-stu-id="d3af2-195">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

<span data-ttu-id="d3af2-196">Você pode usar o exemplo de solicitação e o seguinte corpo de solicitação para atualizar a extensão acima da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="d3af2-196">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="d3af2-197">Alterando `companyName` de `Wingtip Toys` para `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="d3af2-197">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="d3af2-198">Alterando `dealValue` de `500050` para `500100`</span><span class="sxs-lookup"><span data-stu-id="d3af2-198">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="d3af2-199">Adicionar novos dados como a propriedade personalizada `updated`</span><span class="sxs-lookup"><span data-stu-id="d3af2-199">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "Microsoft.Graph.OpenTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="d3af2-200">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="d3af2-200">Response 1</span></span>

<span data-ttu-id="d3af2-201">Aqui está a resposta que é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="d3af2-201">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
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

#### <a name="request-2"></a><span data-ttu-id="d3af2-202">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="d3af2-202">Request 2</span></span>

<span data-ttu-id="d3af2-p109">O segundo exemplo mostra como atualizar uma extensão em uma postagem de grupo. A extensão é representada inicialmente pela seguinte carga JSON, com um valor `expirationDate` de `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="d3af2-p109">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

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

<span data-ttu-id="d3af2-205">A seguir estão a solicitação e o corpo da solicitação para alterar o `expirationDate` para `2016-07-30T11:00:00Z`:</span><span class="sxs-lookup"><span data-stu-id="d3af2-205">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
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

#### <a name="response-2"></a><span data-ttu-id="d3af2-206">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="d3af2-206">Response 2</span></span>

<span data-ttu-id="d3af2-207">Aqui está a resposta do segundo exemplo, que mostra o `expirationDate` atualizado na extensão.</span><span class="sxs-lookup"><span data-stu-id="d3af2-207">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "response",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.opentypeextension"  
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
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
