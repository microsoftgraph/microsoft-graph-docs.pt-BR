---
title: Criar uma configuração de diretório
description: Use essa API para criar uma nova definição, com base em modelos de disponíveis no directorySettingTemplates. Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos). A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que controlam se os membros de um grupo podem convidar usuários convidados pode ser definido. Depois que a capacidade de adicionar usuários convidados a um grupo estiver disponível, isso orientará esse comportamento.
ms.openlocfilehash: 40e90f66c43032deea8ee866b13508fd73c0f17f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035569"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="400d8-107">Criar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="400d8-107">Create a directory setting</span></span>

> <span data-ttu-id="400d8-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="400d8-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="400d8-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="400d8-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="400d8-110">Use essa API para criar uma nova definição, com base em modelos de disponíveis no directorySettingTemplates.</span><span class="sxs-lookup"><span data-stu-id="400d8-110">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="400d8-111">Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos).</span><span class="sxs-lookup"><span data-stu-id="400d8-111">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="400d8-112">A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="400d8-112">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="400d8-113">Para configurações específicas de grupo, somente a configuração que controlam se os membros de um grupo podem convidar usuários convidados pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="400d8-113">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="400d8-114">Depois que a capacidade de adicionar usuários convidados a um grupo estiver disponível, isso orientará esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="400d8-114">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="400d8-115">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="400d8-115">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="400d8-116">A versão de /v1.0 desse API foi renomeada para *criar groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="400d8-116">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="400d8-117">Para obter uma lista de modelos e as propriedades que eles oferecem suporte na versão beta, use uma [consulta directorySettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="400d8-117">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="400d8-118">(Para os pontos de extremidade v 1.0, chamada [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="400d8-118">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="400d8-119">Permissions</span><span class="sxs-lookup"><span data-stu-id="400d8-119">Permissions</span></span>
<span data-ttu-id="400d8-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="400d8-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="400d8-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="400d8-122">Permission type</span></span>      | <span data-ttu-id="400d8-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="400d8-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="400d8-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="400d8-124">Delegated (work or school account)</span></span> | <span data-ttu-id="400d8-125">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="400d8-125">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="400d8-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="400d8-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="400d8-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="400d8-127">Not supported.</span></span>    |
|<span data-ttu-id="400d8-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="400d8-128">Application</span></span> | <span data-ttu-id="400d8-129">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="400d8-129">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="400d8-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="400d8-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="400d8-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="400d8-131">Request headers</span></span>
| <span data-ttu-id="400d8-132">Nome</span><span class="sxs-lookup"><span data-stu-id="400d8-132">Name</span></span>       | <span data-ttu-id="400d8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="400d8-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="400d8-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="400d8-134">Authorization</span></span>  | <span data-ttu-id="400d8-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="400d8-p107">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="400d8-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="400d8-137">Request body</span></span>
<span data-ttu-id="400d8-138">No corpo da solicitação, fornece uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="400d8-138">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="400d8-139">No entanto, o nome de exibição para a configuração será definido com base no nome do modelo de configurações referenciado.</span><span class="sxs-lookup"><span data-stu-id="400d8-139">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="400d8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="400d8-140">Response</span></span>

<span data-ttu-id="400d8-141">Se tiver êxito, este método retornará `201 Created` objeto response de código e [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="400d8-141">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="400d8-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="400d8-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="400d8-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="400d8-143">Request</span></span>
<span data-ttu-id="400d8-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="400d8-144">Here is an example of the request.</span></span>
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
<span data-ttu-id="400d8-145">No corpo da solicitação, fornece uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="400d8-145">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="400d8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="400d8-146">Response</span></span>
<span data-ttu-id="400d8-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="400d8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->