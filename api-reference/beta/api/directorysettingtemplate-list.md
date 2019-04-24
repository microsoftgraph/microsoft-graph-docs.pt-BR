---
title: Listar directorySettingTemplates
description: Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.  Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cd0112bd0d9f98f969832427d497d6e9ba2aa14
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454768"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="f39ee-104">Listar directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="f39ee-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f39ee-105">Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="f39ee-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="f39ee-106">Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f39ee-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="f39ee-107">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="f39ee-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f39ee-108">A versão/v1.0 dessa API foi renomeada para listar *groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="f39ee-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f39ee-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f39ee-109">Permissions</span></span>
<span data-ttu-id="f39ee-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f39ee-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f39ee-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f39ee-112">Permission type</span></span>      | <span data-ttu-id="f39ee-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f39ee-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f39ee-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f39ee-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f39ee-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f39ee-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f39ee-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f39ee-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f39ee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f39ee-117">Not supported.</span></span>    |
|<span data-ttu-id="f39ee-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f39ee-118">Application</span></span> | <span data-ttu-id="f39ee-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f39ee-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f39ee-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f39ee-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f39ee-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f39ee-121">Optional query parameters</span></span>
<span data-ttu-id="f39ee-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f39ee-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f39ee-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f39ee-123">Request headers</span></span>
| <span data-ttu-id="f39ee-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f39ee-124">Name</span></span>      |<span data-ttu-id="f39ee-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f39ee-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f39ee-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f39ee-126">Authorization</span></span>  | <span data-ttu-id="f39ee-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f39ee-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f39ee-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f39ee-129">Request body</span></span>
<span data-ttu-id="f39ee-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f39ee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f39ee-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f39ee-131">Response</span></span>

<span data-ttu-id="f39ee-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f39ee-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f39ee-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f39ee-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f39ee-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f39ee-134">Request</span></span>
<span data-ttu-id="f39ee-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f39ee-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="f39ee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f39ee-136">Response</span></span>
<span data-ttu-id="f39ee-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f39ee-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
