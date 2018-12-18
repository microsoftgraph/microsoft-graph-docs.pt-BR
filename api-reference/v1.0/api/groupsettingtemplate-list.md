---
title: Lista groupSettingTemplates
description: Os Modelos de configuração de grupo representam um conjunto de modelos pelo qual as configurações de grupo podem ser criadas e usadas em um locatário.  Esta operação recupera a lista de objetos groupSettingTemplates disponíveis.
author: dkershaw10
ms.openlocfilehash: b47613093d8efa7fac99a313fff45d846d7a5073
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359357"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="953d7-104">Lista groupSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="953d7-104">List groupSettingTemplates</span></span>

<span data-ttu-id="953d7-p102">Os Modelos de configuração de grupo representam um conjunto de modelos pelo qual as configurações de grupo podem ser criadas e usadas em um locatário.  Esta operação recupera a lista de objetos groupSettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="953d7-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="953d7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="953d7-107">Permissions</span></span>

<span data-ttu-id="953d7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="953d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="953d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="953d7-110">Permission type</span></span>      | <span data-ttu-id="953d7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="953d7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="953d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="953d7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="953d7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="953d7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="953d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="953d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="953d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="953d7-115">Not supported.</span></span>    |
|<span data-ttu-id="953d7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="953d7-116">Application</span></span> | <span data-ttu-id="953d7-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="953d7-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="953d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="953d7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="953d7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="953d7-119">Optional query parameters</span></span>
<span data-ttu-id="953d7-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="953d7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="953d7-121">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="953d7-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="953d7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="953d7-122">Request headers</span></span>
| <span data-ttu-id="953d7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="953d7-123">Name</span></span> | <span data-ttu-id="953d7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="953d7-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="953d7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="953d7-125">Authorization</span></span>  | <span data-ttu-id="953d7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="953d7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="953d7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="953d7-128">Request body</span></span>
<span data-ttu-id="953d7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="953d7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="953d7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="953d7-130">Response</span></span>

<span data-ttu-id="953d7-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="953d7-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="953d7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="953d7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="953d7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="953d7-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="953d7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="953d7-134">Response</span></span>

<span data-ttu-id="953d7-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="953d7-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
                    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
                    "deletedDateTime": null,
                    "displayName": "Group.Unified",
                    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
                    "values": [
                        {
                            "name": "CustomBlockedWordsList",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "EnableMSStandardBlockedWords",
                            "type": "System.Boolean",
                            "defaultValue": "false",
                            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "ClassificationDescriptions",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
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
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->