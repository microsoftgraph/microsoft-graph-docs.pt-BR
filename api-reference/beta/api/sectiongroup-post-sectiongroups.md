---
title: Criar sectionGroup
description: Crie um novo grupo de seção no grupo da seção especificado.
localization_priority: Normal
ms.openlocfilehash: 5af01bd2a526d692b568fe121db7933a2887a006
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812954"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="51822-103">Criar sectionGroup</span><span class="sxs-lookup"><span data-stu-id="51822-103">Create sectionGroup</span></span>

> <span data-ttu-id="51822-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51822-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51822-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51822-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51822-106">Crie um novo [grupo de seção](../resources/sectiongroup.md) no grupo da seção especificado.</span><span class="sxs-lookup"><span data-stu-id="51822-106">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="51822-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="51822-107">Permissions</span></span>
<span data-ttu-id="51822-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51822-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51822-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51822-110">Permission type</span></span>      | <span data-ttu-id="51822-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51822-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51822-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51822-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51822-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51822-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="51822-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51822-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51822-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51822-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="51822-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51822-116">Application</span></span> | <span data-ttu-id="51822-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51822-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51822-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51822-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="51822-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51822-119">Request headers</span></span>
| <span data-ttu-id="51822-120">Nome</span><span class="sxs-lookup"><span data-stu-id="51822-120">Name</span></span>       | <span data-ttu-id="51822-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="51822-121">Type</span></span> | <span data-ttu-id="51822-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="51822-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51822-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51822-123">Authorization</span></span>  | <span data-ttu-id="51822-124">string</span><span class="sxs-lookup"><span data-stu-id="51822-124">string</span></span>  | <span data-ttu-id="51822-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51822-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51822-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51822-127">Content-Type</span></span> | <span data-ttu-id="51822-128">string</span><span class="sxs-lookup"><span data-stu-id="51822-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="51822-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51822-129">Request body</span></span>
<span data-ttu-id="51822-130">No corpo da solicitação, forneça um nome para o grupo de seção.</span><span class="sxs-lookup"><span data-stu-id="51822-130">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="51822-p104">Dentro do mesmo nível de hierarquia, os nomes dos grupos de seção devem ser exclusivos. O nome não pode conter mais de 50 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="51822-p104">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="51822-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="51822-133">Response</span></span>

<span data-ttu-id="51822-134">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51822-134">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51822-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51822-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51822-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51822-136">Request</span></span>
<span data-ttu-id="51822-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51822-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="51822-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="51822-138">Response</span></span>
<span data-ttu-id="51822-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51822-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",  
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
