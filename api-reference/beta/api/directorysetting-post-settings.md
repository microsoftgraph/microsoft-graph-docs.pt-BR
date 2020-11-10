---
title: Criar uma configuração de diretório
description: Use essa API para criar uma nova configuração, com base nos modelos disponíveis no directorySettingTemplates.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d2a94361ee3d92ae6662751a633176ff236819ca
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956174"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="03c64-103">Criar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="03c64-103">Create a directory setting</span></span>

<span data-ttu-id="03c64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03c64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03c64-105">Use essa API para criar uma nova configuração, com base nos modelos disponíveis no directorySettingTemplates.</span><span class="sxs-lookup"><span data-stu-id="03c64-105">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="03c64-106">Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos).</span><span class="sxs-lookup"><span data-stu-id="03c64-106">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="03c64-107">A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="03c64-107">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="03c64-108">Para configurações específicas de grupo, somente a configuração que determina se os membros de um grupo podem convidar usuários convidados podem ser definidos.</span><span class="sxs-lookup"><span data-stu-id="03c64-108">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="03c64-109">Isso irá controlar esse comportamento assim que a capacidade de adicionar usuários convidados a um grupo estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="03c64-109">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="03c64-110">**Observação** : a versão do/beta desta API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="03c64-110">**Note** : The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="03c64-111">A versão/v1.0 dessa API foi renomeada para *criar groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="03c64-111">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="03c64-112">Para obter uma lista de modelos e as propriedades que eles dão suporte na versão beta, use uma [consulta directorySettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="03c64-112">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="03c64-113">(Para pontos de extremidade de v 1.0, chame [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="03c64-113">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="03c64-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="03c64-114">Permissions</span></span>
<span data-ttu-id="03c64-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03c64-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03c64-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03c64-117">Permission type</span></span>      | <span data-ttu-id="03c64-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03c64-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03c64-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03c64-119">Delegated (work or school account)</span></span> | <span data-ttu-id="03c64-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03c64-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03c64-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03c64-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03c64-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03c64-122">Not supported.</span></span>    |
|<span data-ttu-id="03c64-123">Application</span><span class="sxs-lookup"><span data-stu-id="03c64-123">Application</span></span> | <span data-ttu-id="03c64-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03c64-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03c64-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03c64-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="03c64-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03c64-126">Request headers</span></span>
| <span data-ttu-id="03c64-127">Nome</span><span class="sxs-lookup"><span data-stu-id="03c64-127">Name</span></span>       | <span data-ttu-id="03c64-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="03c64-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03c64-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="03c64-129">Authorization</span></span>  | <span data-ttu-id="03c64-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03c64-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03c64-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03c64-132">Request body</span></span>
<span data-ttu-id="03c64-133">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="03c64-133">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="03c64-134">No entanto, o nome de exibição da configuração será definido com base no nome do modelo de configurações referenciado.</span><span class="sxs-lookup"><span data-stu-id="03c64-134">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="03c64-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="03c64-135">Response</span></span>

<span data-ttu-id="03c64-136">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03c64-136">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03c64-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03c64-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03c64-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03c64-138">Request</span></span>
<span data-ttu-id="03c64-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03c64-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03c64-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="03c64-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="03c64-141">C#</span><span class="sxs-lookup"><span data-stu-id="03c64-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03c64-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03c64-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03c64-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03c64-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03c64-144">Java</span><span class="sxs-lookup"><span data-stu-id="03c64-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directorysetting-from-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="03c64-145">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="03c64-145">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="03c64-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="03c64-146">Response</span></span>
<span data-ttu-id="03c64-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03c64-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


