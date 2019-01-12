---
title: Atualizar propriedades educationclass
description: Atualize as propriedades de uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7932dc3072689468ceff813a99466d287ce77a1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950561"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="1bcd5-103">Atualizar propriedades educationclass</span><span class="sxs-lookup"><span data-stu-id="1bcd5-103">Update educationclass properties</span></span>

> <span data-ttu-id="1bcd5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bcd5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1bcd5-106">Atualize as propriedades de uma aula.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-106">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bcd5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bcd5-107">Permissions</span></span>
<span data-ttu-id="1bcd5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bcd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bcd5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bcd5-110">Permission type</span></span>      | <span data-ttu-id="1bcd5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bcd5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bcd5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bcd5-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="1bcd5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-113">Not supported.</span></span>  |
|<span data-ttu-id="1bcd5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bcd5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bcd5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-115">Not supported.</span></span>   |
|<span data-ttu-id="1bcd5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bcd5-116">Application</span></span> | <span data-ttu-id="1bcd5-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bcd5-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1bcd5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bcd5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1bcd5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcd5-119">Request headers</span></span>
| <span data-ttu-id="1bcd5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bcd5-120">Header</span></span>       | <span data-ttu-id="1bcd5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1bcd5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bcd5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bcd5-122">Authorization</span></span>  | <span data-ttu-id="1bcd5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1bcd5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1bcd5-125">Content-Type</span></span>  | <span data-ttu-id="1bcd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bcd5-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bcd5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcd5-127">Request body</span></span>
<span data-ttu-id="1bcd5-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1bcd5-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1bcd5-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1bcd5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bcd5-131">Property</span></span>     | <span data-ttu-id="1bcd5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bcd5-132">Type</span></span>   |<span data-ttu-id="1bcd5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bcd5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bcd5-134">description</span><span class="sxs-lookup"><span data-stu-id="1bcd5-134">description</span></span>|<span data-ttu-id="1bcd5-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bcd5-135">String</span></span>| <span data-ttu-id="1bcd5-136">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-136">Description of the class.</span></span>|
|<span data-ttu-id="1bcd5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1bcd5-137">displayName</span></span>|<span data-ttu-id="1bcd5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bcd5-138">String</span></span>| <span data-ttu-id="1bcd5-139">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-139">Name of the class.</span></span>|
|<span data-ttu-id="1bcd5-140">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1bcd5-140">mailNickname</span></span>|<span data-ttu-id="1bcd5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bcd5-141">String</span></span>| <span data-ttu-id="1bcd5-142">Alias de email para envio de email a todos os usuários, se esse recurso estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-142">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="1bcd5-143"><!-- Please verify the revised description here. -->| classCode | Cadeia de caracteres | Classe de código usado pelo escola. | | externalId | Cadeia de caracteres | ID da classe do sistema sincronizando.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-143"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="1bcd5-144">| |externalName|Cadeia de caracteres|Nome da aula no sistema de sincronização.| |externalSource|cadeia de caracteres| Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-144">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="1bcd5-145">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.|</span><span class="sxs-lookup"><span data-stu-id="1bcd5-145">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="1bcd5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bcd5-146">Response</span></span>
<span data-ttu-id="1bcd5-147">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-147">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bcd5-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bcd5-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bcd5-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bcd5-149">Request</span></span>
<span data-ttu-id="1bcd5-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="1bcd5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bcd5-151">Response</span></span>
<span data-ttu-id="1bcd5-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-152">The following is an example of the response.</span></span> 

><span data-ttu-id="1bcd5-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bcd5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
