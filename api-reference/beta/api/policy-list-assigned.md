---
title: Listar políticas atribuídas à entidade de serviço ou aplicativo
description: Obter os objetos de política atribuídos a uma entidade de serviço ou aplicativo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 12e252067c7f7c8672543292a65b8650a43d45c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455512"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="ccad4-103">Listar políticas atribuídas à entidade de serviço ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccad4-103">List Policies assigned to Application or Service Principal</span></span>

<span data-ttu-id="ccad4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ccad4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccad4-105">Obter os objetos de [política](../resources/policy.md) atribuídos a uma entidade de serviço ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ccad4-105">Get the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccad4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccad4-106">Permissions</span></span>
<span data-ttu-id="ccad4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccad4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccad4-109">Permission type</span></span>      | <span data-ttu-id="ccad4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccad4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccad4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccad4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ccad4-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ccad4-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ccad4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccad4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccad4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccad4-114">Not supported.</span></span>    |
|<span data-ttu-id="ccad4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccad4-115">Application</span></span> | <span data-ttu-id="ccad4-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccad4-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccad4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccad4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="ccad4-118">Observação: "ID" na solicitação é a propriedade "ID" da entidade de serviço ou aplicativo, não a propriedade "AppID".</span><span class="sxs-lookup"><span data-stu-id="ccad4-118">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccad4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccad4-119">Request headers</span></span>
| <span data-ttu-id="ccad4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ccad4-120">Name</span></span>       | <span data-ttu-id="ccad4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccad4-121">Type</span></span> | <span data-ttu-id="ccad4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccad4-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ccad4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccad4-123">Authorization</span></span>  | <span data-ttu-id="ccad4-124">string</span><span class="sxs-lookup"><span data-stu-id="ccad4-124">string</span></span>  | <span data-ttu-id="ccad4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccad4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccad4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccad4-127">Request body</span></span>
<span data-ttu-id="ccad4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ccad4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccad4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccad4-129">Response</span></span>

<span data-ttu-id="ccad4-130">Se bem-sucedido, este método retorna `200 OK` o código de resposta e os objetos [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccad4-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="ccad4-131">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="ccad4-131">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ccad4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccad4-132">Example</span></span>
<span data-ttu-id="ccad4-133">O exemplo a seguir recupera as políticas atribuídas a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ccad4-133">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="ccad4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccad4-134">Request</span></span>
<span data-ttu-id="ccad4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccad4-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="ccad4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccad4-136">Response</span></span>
<span data-ttu-id="ccad4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccad4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
