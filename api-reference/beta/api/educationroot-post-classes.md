---
title: Criar educationClass
description: Crie uma nova aula. Isso também criará um grupo universal. Quando você usa essa API para criar uma classe, ele adicionará propriedades especiais para o grupo, que será
localization_priority: Normal
ms.openlocfilehash: b75ce58b1d56fe1ba231299b9c2c943ca28e0403
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843467"
---
# <a name="create-educationclass"></a><span data-ttu-id="21d7e-105">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="21d7e-105">Create educationClass</span></span>

> <span data-ttu-id="21d7e-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21d7e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21d7e-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21d7e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21d7e-108">Crie uma nova aula.</span><span class="sxs-lookup"><span data-stu-id="21d7e-108">Create a new class.</span></span> <span data-ttu-id="21d7e-109">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="21d7e-109">This will also create a universal group.</span></span> <span data-ttu-id="21d7e-110">Quando você usar essa API para criar uma aula, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="21d7e-110">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="21d7e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="21d7e-111">Permissions</span></span>
<span data-ttu-id="21d7e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21d7e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21d7e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21d7e-114">Permission type</span></span>      | <span data-ttu-id="21d7e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21d7e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21d7e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21d7e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="21d7e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21d7e-117">Not supported.</span></span>  |
|<span data-ttu-id="21d7e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21d7e-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="21d7e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21d7e-119">Not supported.</span></span>  |
|<span data-ttu-id="21d7e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21d7e-120">Application</span></span> | <span data-ttu-id="21d7e-121">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d7e-121">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="21d7e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21d7e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="21d7e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21d7e-123">Request headers</span></span>
| <span data-ttu-id="21d7e-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21d7e-124">Header</span></span>       | <span data-ttu-id="21d7e-125">Valor</span><span class="sxs-lookup"><span data-stu-id="21d7e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21d7e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="21d7e-126">Authorization</span></span>  | <span data-ttu-id="21d7e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21d7e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="21d7e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21d7e-129">Content-Type</span></span>  | <span data-ttu-id="21d7e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="21d7e-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21d7e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21d7e-131">Request body</span></span>
<span data-ttu-id="21d7e-132">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="21d7e-132">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="21d7e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="21d7e-133">Response</span></span>
<span data-ttu-id="21d7e-134">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21d7e-134">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21d7e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21d7e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21d7e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21d7e-136">Request</span></span>
<span data-ttu-id="21d7e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21d7e-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```

##### <a name="response"></a><span data-ttu-id="21d7e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="21d7e-138">Response</span></span>
<span data-ttu-id="21d7e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21d7e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="21d7e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21d7e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

{
    "id": "11019",
    "description": "Health Level 1",
    "classCode": "Health 501",
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012",
      }
    },
    "displayName": "Health 1",
    "externalId": "11019",
    "externalName": "Health Level 1",
    "externalSource": "sis",
    "mailNickname": "fineartschool.net"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
