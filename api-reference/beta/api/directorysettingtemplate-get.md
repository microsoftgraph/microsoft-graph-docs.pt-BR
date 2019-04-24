---
title: Obter um modelo de configuração de diretório
description: Um modelo de configuração de diretório representa um modelo de configurações das quais as configurações podem ser criadas em um locatário. Essa operação permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus padrões.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c097d9919a52cde8559ead338f433b27a1e3e73d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454936"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="464ec-104">Obter um modelo de configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="464ec-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="464ec-105">Um modelo de configuração de diretório representa um modelo de configurações das quais as configurações podem ser criadas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="464ec-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="464ec-106">Essa operação permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="464ec-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="464ec-107">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="464ec-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="464ec-108">A versão do/v1.0 dessa API foi renomeada para *obter groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="464ec-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="464ec-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="464ec-109">Permissions</span></span>
<span data-ttu-id="464ec-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="464ec-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="464ec-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="464ec-112">Permission type</span></span>      | <span data-ttu-id="464ec-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="464ec-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="464ec-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="464ec-114">Delegated (work or school account)</span></span> | <span data-ttu-id="464ec-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="464ec-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="464ec-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="464ec-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="464ec-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="464ec-117">Not supported.</span></span>    |
|<span data-ttu-id="464ec-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="464ec-118">Application</span></span> | <span data-ttu-id="464ec-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="464ec-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="464ec-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="464ec-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="464ec-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="464ec-121">Optional query parameters</span></span>
<span data-ttu-id="464ec-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="464ec-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="464ec-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="464ec-123">Request headers</span></span>
| <span data-ttu-id="464ec-124">Nome</span><span class="sxs-lookup"><span data-stu-id="464ec-124">Name</span></span>      |<span data-ttu-id="464ec-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="464ec-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="464ec-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="464ec-126">Authorization</span></span>  | <span data-ttu-id="464ec-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="464ec-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="464ec-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="464ec-129">Request body</span></span>
<span data-ttu-id="464ec-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="464ec-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="464ec-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="464ec-131">Response</span></span>

<span data-ttu-id="464ec-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="464ec-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="464ec-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="464ec-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="464ec-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="464ec-134">Request</span></span>
<span data-ttu-id="464ec-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="464ec-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="464ec-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="464ec-136">Response</span></span>
<span data-ttu-id="464ec-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="464ec-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 270

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
  ],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
