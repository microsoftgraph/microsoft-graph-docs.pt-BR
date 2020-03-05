---
title: Criar uma configuração de diretório
description: Use essa API para criar uma nova configuração, com base nos modelos disponíveis no directorySettingTemplates. Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos). A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que determina se os membros de um grupo podem convidar usuários convidados podem ser definidos. Isso irá controlar esse comportamento assim que a capacidade de adicionar usuários convidados a um grupo estiver disponível.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b88e405d8850eef49fd73fff792a94cf727863a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433969"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="8f969-107">Criar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="8f969-107">Create a directory setting</span></span>

<span data-ttu-id="8f969-108">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8f969-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f969-109">Use essa API para criar uma nova configuração, com base nos modelos disponíveis no directorySettingTemplates.</span><span class="sxs-lookup"><span data-stu-id="8f969-109">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="8f969-110">Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos).</span><span class="sxs-lookup"><span data-stu-id="8f969-110">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="8f969-111">A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="8f969-111">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="8f969-112">Para configurações específicas de grupo, somente a configuração que determina se os membros de um grupo podem convidar usuários convidados podem ser definidos.</span><span class="sxs-lookup"><span data-stu-id="8f969-112">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="8f969-113">Isso irá controlar esse comportamento assim que a capacidade de adicionar usuários convidados a um grupo estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="8f969-113">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="8f969-114">**Observação**: a versão do/beta desta API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="8f969-114">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="8f969-115">A versão/v1.0 dessa API foi renomeada para *criar groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="8f969-115">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="8f969-116">Para obter uma lista de modelos e as propriedades que eles dão suporte na versão beta, use uma [consulta directorySettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="8f969-116">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="8f969-117">(Para pontos de extremidade de v 1.0, chame [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="8f969-117">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="8f969-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f969-118">Permissions</span></span>
<span data-ttu-id="8f969-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f969-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f969-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f969-121">Permission type</span></span>      | <span data-ttu-id="8f969-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f969-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f969-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f969-123">Delegated (work or school account)</span></span> | <span data-ttu-id="8f969-124">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8f969-124">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8f969-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f969-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f969-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f969-126">Not supported.</span></span>    |
|<span data-ttu-id="8f969-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f969-127">Application</span></span> | <span data-ttu-id="8f969-128">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f969-128">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f969-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f969-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="8f969-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f969-130">Request headers</span></span>
| <span data-ttu-id="8f969-131">Nome</span><span class="sxs-lookup"><span data-stu-id="8f969-131">Name</span></span>       | <span data-ttu-id="8f969-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f969-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f969-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f969-133">Authorization</span></span>  | <span data-ttu-id="8f969-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f969-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f969-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f969-136">Request body</span></span>
<span data-ttu-id="8f969-137">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="8f969-137">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="8f969-138">No entanto, o nome de exibição da configuração será definido com base no nome do modelo de configurações referenciado.</span><span class="sxs-lookup"><span data-stu-id="8f969-138">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="8f969-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f969-139">Response</span></span>

<span data-ttu-id="8f969-140">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f969-140">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f969-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f969-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f969-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f969-142">Request</span></span>
<span data-ttu-id="8f969-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f969-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f969-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f969-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8f969-145">C#</span><span class="sxs-lookup"><span data-stu-id="8f969-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f969-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f969-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f969-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f969-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8f969-148">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="8f969-148">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8f969-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f969-149">Response</span></span>
<span data-ttu-id="8f969-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f969-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
