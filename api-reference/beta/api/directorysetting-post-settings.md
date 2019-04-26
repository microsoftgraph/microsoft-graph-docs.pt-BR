---
title: Criar uma configuração de diretório
description: Use essa API para criar uma nova configuração, com base nos modelos disponíveis no directorySettingTemplates. Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos). A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que determina se os membros de um grupo podem convidar usuários convidados podem ser definidos. Isso irá controlar esse comportamento assim que a capacidade de adicionar usuários convidados a um grupo estiver disponível.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 097fdc26dd78986e6a869a26e214d073db03f98b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325818"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="b16d6-107">Criar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="b16d6-107">Create a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b16d6-108">Use essa API para criar uma nova configuração, com base nos modelos disponíveis no directorySettingTemplates.</span><span class="sxs-lookup"><span data-stu-id="b16d6-108">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="b16d6-109">Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos).</span><span class="sxs-lookup"><span data-stu-id="b16d6-109">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="b16d6-110">A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="b16d6-110">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="b16d6-111">Para configurações específicas de grupo, somente a configuração que determina se os membros de um grupo podem convidar usuários convidados podem ser definidos.</span><span class="sxs-lookup"><span data-stu-id="b16d6-111">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="b16d6-112">Isso irá controlar esse comportamento assim que a capacidade de adicionar usuários convidados a um grupo estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="b16d6-112">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="b16d6-113">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="b16d6-113">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="b16d6-114">A versão/v1.0 dessa API foi renomeada para *criar groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="b16d6-114">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="b16d6-115">Para obter uma lista de modelos e as propriedades que eles dão suporte na versão beta, use uma [consulta directorySettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="b16d6-115">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="b16d6-116">(Para pontos de extremidade de v 1.0, chame [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="b16d6-116">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="b16d6-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="b16d6-117">Permissions</span></span>
<span data-ttu-id="b16d6-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b16d6-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b16d6-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b16d6-120">Permission type</span></span>      | <span data-ttu-id="b16d6-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b16d6-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b16d6-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b16d6-122">Delegated (work or school account)</span></span> | <span data-ttu-id="b16d6-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b16d6-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b16d6-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b16d6-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b16d6-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b16d6-125">Not supported.</span></span>    |
|<span data-ttu-id="b16d6-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b16d6-126">Application</span></span> | <span data-ttu-id="b16d6-127">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b16d6-127">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b16d6-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b16d6-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="b16d6-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b16d6-129">Request headers</span></span>
| <span data-ttu-id="b16d6-130">Nome</span><span class="sxs-lookup"><span data-stu-id="b16d6-130">Name</span></span>       | <span data-ttu-id="b16d6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b16d6-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b16d6-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b16d6-132">Authorization</span></span>  | <span data-ttu-id="b16d6-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b16d6-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b16d6-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b16d6-135">Request body</span></span>
<span data-ttu-id="b16d6-136">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="b16d6-136">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="b16d6-137">No enTanto, o nome de exibição da configuração será definido com base no nome do modelo de configurações referenciado.</span><span class="sxs-lookup"><span data-stu-id="b16d6-137">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="b16d6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b16d6-138">Response</span></span>

<span data-ttu-id="b16d6-139">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b16d6-139">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b16d6-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b16d6-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b16d6-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b16d6-141">Request</span></span>
<span data-ttu-id="b16d6-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b16d6-142">Here is an example of the request.</span></span>
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
<span data-ttu-id="b16d6-143">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="b16d6-143">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b16d6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b16d6-144">Response</span></span>
<span data-ttu-id="b16d6-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b16d6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
