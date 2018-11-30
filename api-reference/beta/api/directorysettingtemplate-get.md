---
title: Obter um modelo de configuração de diretório
description: Um modelo de configuração de diretório representa um modelo de configurações do qual as configurações podem ser criadas em um locatário. Essa operação permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus valores padrão.
ms.openlocfilehash: 1928642883632a672ddaccb9181f6366ade5ce04
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033648"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="d83f9-104">Obter um modelo de configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="d83f9-104">Get a directory setting template</span></span>

> <span data-ttu-id="d83f9-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d83f9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d83f9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d83f9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d83f9-107">Um modelo de configuração de diretório representa um modelo de configurações do qual as configurações podem ser criadas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="d83f9-107">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="d83f9-108">Essa operação permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus valores padrão.</span><span class="sxs-lookup"><span data-stu-id="d83f9-108">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="d83f9-109">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="d83f9-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d83f9-110">A versão de /v1.0 desse API foi renomeada para *obter groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="d83f9-110">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d83f9-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="d83f9-111">Permissions</span></span>
<span data-ttu-id="d83f9-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d83f9-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d83f9-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d83f9-114">Permission type</span></span>      | <span data-ttu-id="d83f9-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d83f9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d83f9-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d83f9-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d83f9-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d83f9-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d83f9-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d83f9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d83f9-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d83f9-119">Not supported.</span></span>    |
|<span data-ttu-id="d83f9-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d83f9-120">Application</span></span> | <span data-ttu-id="d83f9-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d83f9-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d83f9-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d83f9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d83f9-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d83f9-123">Optional query parameters</span></span>
<span data-ttu-id="d83f9-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d83f9-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d83f9-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d83f9-125">Request headers</span></span>
| <span data-ttu-id="d83f9-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d83f9-126">Name</span></span>      |<span data-ttu-id="d83f9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d83f9-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d83f9-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d83f9-128">Authorization</span></span>  | <span data-ttu-id="d83f9-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d83f9-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d83f9-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d83f9-131">Request body</span></span>
<span data-ttu-id="d83f9-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d83f9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d83f9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d83f9-133">Response</span></span>

<span data-ttu-id="d83f9-134">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d83f9-134">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d83f9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d83f9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d83f9-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d83f9-136">Request</span></span>
<span data-ttu-id="d83f9-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d83f9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="d83f9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d83f9-138">Response</span></span>
<span data-ttu-id="d83f9-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d83f9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->