---
title: Lista directorySettingTemplates
description: A definição de modelos de diretório representa um conjunto de modelos de configurações de diretório, do qual directory configurações podem ser criadas e usadas em um locatário.  Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.
localization_priority: Normal
ms.openlocfilehash: 288a914da11c09cd39767a48d527510998c9be1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833324"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="f2acd-104">Lista directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="f2acd-104">List directorySettingTemplates</span></span>

> <span data-ttu-id="f2acd-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2acd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2acd-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2acd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2acd-107">A definição de modelos de diretório representa um conjunto de modelos de configurações de diretório, do qual directory configurações podem ser criadas e usadas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="f2acd-107">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="f2acd-108">Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f2acd-108">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="f2acd-109">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="f2acd-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f2acd-110">A versão de /v1.0 desse API foi renomeada para *groupSettingTemplate de lista*.</span><span class="sxs-lookup"><span data-stu-id="f2acd-110">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2acd-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="f2acd-111">Permissions</span></span>
<span data-ttu-id="f2acd-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2acd-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2acd-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2acd-114">Permission type</span></span>      | <span data-ttu-id="f2acd-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2acd-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2acd-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2acd-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f2acd-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2acd-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2acd-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2acd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2acd-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2acd-119">Not supported.</span></span>    |
|<span data-ttu-id="f2acd-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2acd-120">Application</span></span> | <span data-ttu-id="f2acd-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2acd-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2acd-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2acd-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f2acd-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2acd-123">Optional query parameters</span></span>
<span data-ttu-id="f2acd-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2acd-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2acd-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2acd-125">Request headers</span></span>
| <span data-ttu-id="f2acd-126">Nome</span><span class="sxs-lookup"><span data-stu-id="f2acd-126">Name</span></span>      |<span data-ttu-id="f2acd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2acd-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2acd-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2acd-128">Authorization</span></span>  | <span data-ttu-id="f2acd-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2acd-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2acd-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2acd-131">Request body</span></span>
<span data-ttu-id="f2acd-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2acd-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2acd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2acd-133">Response</span></span>

<span data-ttu-id="f2acd-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2acd-134">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2acd-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2acd-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2acd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2acd-136">Request</span></span>
<span data-ttu-id="f2acd-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2acd-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="f2acd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2acd-138">Response</span></span>
<span data-ttu-id="f2acd-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2acd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "description": "description-value",
      "values": [
        {
          "name": "name-value",
          "type": "type-value",
          "defaultValue": "defaultValue-value",
          "description": "description-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
