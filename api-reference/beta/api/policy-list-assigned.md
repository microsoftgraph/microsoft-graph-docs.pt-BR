---
title: Políticas de lista atribuídas ao aplicativo ou entidade de serviço
description: Recupere os objetos de política atribuídos a um aplicativo ou entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 3c66eece645313f7039f12aec708cba4581fb4bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875352"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="a6241-103">Políticas de lista atribuídas ao aplicativo ou entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="a6241-103">List Policies assigned to Application or Service Principal</span></span>

> <span data-ttu-id="a6241-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6241-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6241-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6241-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6241-106">Recupere os objetos de [política](../resources/policy.md) atribuídos a um aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="a6241-106">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6241-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a6241-107">Permissions</span></span>
<span data-ttu-id="a6241-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6241-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6241-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6241-110">Permission type</span></span>      | <span data-ttu-id="a6241-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6241-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6241-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6241-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6241-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6241-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a6241-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6241-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6241-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6241-115">Not supported.</span></span>    |
|<span data-ttu-id="a6241-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6241-116">Application</span></span> | <span data-ttu-id="a6241-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6241-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6241-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6241-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="a6241-119">Observação: O "id" na solicitação é a propriedade "id" do aplicativo ou serviço principal, não a propriedade "appid".</span><span class="sxs-lookup"><span data-stu-id="a6241-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6241-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6241-120">Request headers</span></span>
| <span data-ttu-id="a6241-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a6241-121">Name</span></span>       | <span data-ttu-id="a6241-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6241-122">Type</span></span> | <span data-ttu-id="a6241-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6241-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6241-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6241-124">Authorization</span></span>  | <span data-ttu-id="a6241-125">string</span><span class="sxs-lookup"><span data-stu-id="a6241-125">string</span></span>  | <span data-ttu-id="a6241-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6241-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6241-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6241-128">Request body</span></span>
<span data-ttu-id="a6241-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6241-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6241-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6241-130">Response</span></span>

<span data-ttu-id="a6241-131">Se tiver êxito, este método retornará `200 OK` objetos de código e a [diretiva](../resources/policy.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6241-131">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="a6241-132">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="a6241-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="a6241-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6241-133">Example</span></span>
<span data-ttu-id="a6241-134">O exemplo a seguir recupera as políticas atribuídas a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6241-134">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="a6241-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6241-135">Request</span></span>
<span data-ttu-id="a6241-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6241-136">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="a6241-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6241-137">Response</span></span>
<span data-ttu-id="a6241-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6241-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
