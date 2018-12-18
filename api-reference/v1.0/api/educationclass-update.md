---
title: Atualizar propriedades educationclass
description: Atualize as propriedades de uma aula.
author: mmast-msft
ms.openlocfilehash: 9a11ae5e1a2139df4ade3417c940d00dea2d1888
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358706"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="8f866-103">Atualizar propriedades educationclass</span><span class="sxs-lookup"><span data-stu-id="8f866-103">Update educationclass properties</span></span>

<span data-ttu-id="8f866-104">Atualize as propriedades de uma aula.</span><span class="sxs-lookup"><span data-stu-id="8f866-104">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f866-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f866-105">Permissions</span></span>
<span data-ttu-id="8f866-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f866-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f866-108">Permission type</span></span>      | <span data-ttu-id="8f866-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f866-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f866-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f866-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8f866-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f866-111">Not supported.</span></span>  |
|<span data-ttu-id="8f866-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f866-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f866-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f866-113">Not supported.</span></span>   |
|<span data-ttu-id="8f866-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f866-114">Application</span></span> | <span data-ttu-id="8f866-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f866-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8f866-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f866-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8f866-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f866-117">Request headers</span></span>
| <span data-ttu-id="8f866-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f866-118">Header</span></span>       | <span data-ttu-id="8f866-119">Valor</span><span class="sxs-lookup"><span data-stu-id="8f866-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8f866-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f866-120">Authorization</span></span>  | <span data-ttu-id="8f866-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f866-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8f866-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f866-123">Content-Type</span></span>  | <span data-ttu-id="8f866-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f866-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f866-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f866-125">Request body</span></span>
<span data-ttu-id="8f866-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8f866-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8f866-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8f866-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8f866-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8f866-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8f866-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f866-129">Property</span></span>     | <span data-ttu-id="8f866-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f866-130">Type</span></span>   |<span data-ttu-id="8f866-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f866-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f866-132">description</span><span class="sxs-lookup"><span data-stu-id="8f866-132">description</span></span>|<span data-ttu-id="8f866-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f866-133">String</span></span>| <span data-ttu-id="8f866-134">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="8f866-134">Description of the class.</span></span>|
|<span data-ttu-id="8f866-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8f866-135">displayName</span></span>|<span data-ttu-id="8f866-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f866-136">String</span></span>| <span data-ttu-id="8f866-137">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="8f866-137">Name of the class.</span></span>|
|<span data-ttu-id="8f866-138">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8f866-138">mailNickname</span></span>|<span data-ttu-id="8f866-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f866-139">String</span></span>| <span data-ttu-id="8f866-140">Alias de email para envio de email a todos os usuários, se esse recurso estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="8f866-140">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="8f866-141"><!-- Please verify the revised description here. -->| classCode | Cadeia de caracteres | Classe de código usado pelo escola. | | externalId | Cadeia de caracteres | ID da classe do sistema sincronizando.</span><span class="sxs-lookup"><span data-stu-id="8f866-141"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="8f866-142">| |externalName|Cadeia de caracteres|Nome da aula no sistema de sincronização.| |externalSource|cadeia de caracteres| Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="8f866-142">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="8f866-143">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`. |</span><span class="sxs-lookup"><span data-stu-id="8f866-143">The possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="8f866-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f866-144">Response</span></span>
<span data-ttu-id="8f866-145">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f866-145">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f866-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f866-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f866-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f866-147">Request</span></span>
<span data-ttu-id="8f866-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f866-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/{class-id}
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="8f866-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f866-149">Response</span></span>
<span data-ttu-id="8f866-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f866-150">The following is an example of the response.</span></span> 

><span data-ttu-id="8f866-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f866-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->