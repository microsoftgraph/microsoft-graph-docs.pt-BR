---
title: Obter educationClass
description: "  grupo Administradores representam os professores na classe. Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros."
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: ddf29c9d2a136f8f5cee24b30ef9ab1c0f9643f5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935679"
---
# <a name="get-educationclass"></a><span data-ttu-id="e9023-104">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="e9023-104">Get educationClass</span></span>

> <span data-ttu-id="e9023-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e9023-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9023-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e9023-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9023-107">Recupere uma aula do sistema.</span><span class="sxs-lookup"><span data-stu-id="e9023-107">Retrieve a class from the system.</span></span> <span data-ttu-id="e9023-108">Uma aula é um grupo universal com uma propriedade especial que indica ao sistema que o grupo é uma aula.</span><span class="sxs-lookup"><span data-stu-id="e9023-108">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="e9023-109">Os membros do grupo representam os alunos; os administradores do grupo representam os professores da aula.</span><span class="sxs-lookup"><span data-stu-id="e9023-109">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="e9023-110">Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros.</span><span class="sxs-lookup"><span data-stu-id="e9023-110">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9023-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9023-111">Permissions</span></span>
<span data-ttu-id="e9023-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9023-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9023-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9023-114">Permission type</span></span>      | <span data-ttu-id="e9023-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9023-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9023-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9023-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="e9023-117">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e9023-117">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="e9023-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9023-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e9023-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e9023-119">Not supported</span></span>  |
|<span data-ttu-id="e9023-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9023-120">Application</span></span> | <span data-ttu-id="e9023-121">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9023-121">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e9023-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9023-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9023-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9023-123">Optional query parameters</span></span>
<span data-ttu-id="e9023-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9023-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9023-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9023-125">Request headers</span></span>
| <span data-ttu-id="e9023-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9023-126">Header</span></span>       | <span data-ttu-id="e9023-127">Valor</span><span class="sxs-lookup"><span data-stu-id="e9023-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9023-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9023-128">Authorization</span></span>  | <span data-ttu-id="e9023-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9023-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9023-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9023-131">Request body</span></span>
<span data-ttu-id="e9023-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9023-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e9023-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9023-133">Response</span></span>
<span data-ttu-id="e9023-134">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9023-134">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9023-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9023-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9023-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9023-136">Request</span></span>
<span data-ttu-id="e9023-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9023-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023
```
##### <a name="response"></a><span data-ttu-id="e9023-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9023-138">Response</span></span>
<span data-ttu-id="e9023-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9023-139">The following is an example of the response.</span></span> 

><span data-ttu-id="e9023-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9023-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
