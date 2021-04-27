---
title: Atualizar relatedContacts
description: Atualize a coleção relatedContact de um objeto educationUser.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 25c3655318ef063d702f328f008441653437945e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052863"
---
# <a name="update-relatedcontacts"></a><span data-ttu-id="96627-103">Atualizar relatedContacts</span><span class="sxs-lookup"><span data-stu-id="96627-103">Update relatedContacts</span></span>

<span data-ttu-id="96627-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96627-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96627-105">Atualize [a coleção relatedContact](../resources/relatedContact.md) de um [objeto educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="96627-105">Update the [relatedContact](../resources/relatedContact.md) collection of an [educationUser](../resources/educationuser.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="96627-106">A atualização **de relatedContacts** substitui toda a coleção.</span><span class="sxs-lookup"><span data-stu-id="96627-106">Updating **relatedContacts** replaces the entire collection.</span></span> <span data-ttu-id="96627-107">Não é possível adicionar, remover ou atualizar um único contato.</span><span class="sxs-lookup"><span data-stu-id="96627-107">It is not possible to add, remove, or update a single contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="96627-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="96627-108">Permissions</span></span>

<span data-ttu-id="96627-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96627-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96627-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96627-111">Permission type</span></span>                        | <span data-ttu-id="96627-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96627-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="96627-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96627-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="96627-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96627-114">Not supported.</span></span>                              |
| <span data-ttu-id="96627-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96627-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96627-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96627-116">Not supported.</span></span>                              |
| <span data-ttu-id="96627-117">Application</span><span class="sxs-lookup"><span data-stu-id="96627-117">Application</span></span>                            | <span data-ttu-id="96627-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96627-118">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="96627-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96627-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96627-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96627-120">Request headers</span></span>

| <span data-ttu-id="96627-121">Nome</span><span class="sxs-lookup"><span data-stu-id="96627-121">Name</span></span>          | <span data-ttu-id="96627-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="96627-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="96627-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96627-123">Authorization</span></span> | <span data-ttu-id="96627-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96627-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="96627-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96627-126">Content-Type</span></span>  | <span data-ttu-id="96627-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96627-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96627-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96627-129">Request body</span></span>

<span data-ttu-id="96627-130">No corpo da solicitação, fornece uma representação JSON da [coleção relatedContact.](../resources/relatedcontact.md)</span><span class="sxs-lookup"><span data-stu-id="96627-130">In the request body, supply a JSON representation of the [relatedContact](../resources/relatedcontact.md) collection.</span></span>

<span data-ttu-id="96627-131">A tabela a seguir mostra as propriedades necessárias ao atualizar [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="96627-131">The following table shows the properties that are required when you update the [educationUser](../resources/educationuser.md).</span></span>

| <span data-ttu-id="96627-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96627-132">Property</span></span>        | <span data-ttu-id="96627-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="96627-133">Type</span></span>                                                        | <span data-ttu-id="96627-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="96627-134">Description</span></span>                                    |
| :-------------- | :---------------------------------------------------------- | :--------------------------------------------- |
| <span data-ttu-id="96627-135">relatedContacts</span><span class="sxs-lookup"><span data-stu-id="96627-135">relatedContacts</span></span> | <span data-ttu-id="96627-136">[coleção relatedContact](../resources/relatedcontact.md)</span><span class="sxs-lookup"><span data-stu-id="96627-136">[relatedContact](../resources/relatedcontact.md) collection</span></span> | <span data-ttu-id="96627-137">O conjunto completo de contatos relacionados para um usuário</span><span class="sxs-lookup"><span data-stu-id="96627-137">The complete set of related contact for a user</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="96627-138">Essa atualização deve ser uma operação distinta.</span><span class="sxs-lookup"><span data-stu-id="96627-138">This update must be a distinct operation.</span></span> <span data-ttu-id="96627-139">Ele não pode ser combinado com atualizações para outras propriedades [educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="96627-139">It cannot be combined with updates to other [educationUser](../resources/educationuser.md) properties.</span></span>
> <span data-ttu-id="96627-140">Por exemplo, a atualização de **Ambos osContacts relacionados** e **displayName** requer duas solicitações distintas.</span><span class="sxs-lookup"><span data-stu-id="96627-140">For example, updating both **relatedContacts** and **displayName** requires two distinct requests.</span></span>

## <a name="response"></a><span data-ttu-id="96627-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="96627-141">Response</span></span>

<span data-ttu-id="96627-142">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96627-142">If successful, this method returns a `200 OK` response code and an updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96627-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="96627-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96627-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96627-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="96627-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="96627-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}
-->

```http
PATCH https://graph.microsoft.com/beta/education/users/{educationUserId}
Content-Type: application/json
Content-length: 408

{
  "relatedContacts": [
    {
      "displayName": "Father Time",
      "emailAddress": "father@time.com",
      "mobilePhone": "4251231234",
      "relationship": "guardian",
      "accessConsent": true
    },
    {
      "displayName": "Mother Nature",
      "emailAddress": "mother@nature.co.uk",
      "mobilePhone": "3251231234",
      "relationship": "parent",
      "accessConsent": true
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="96627-146">C#</span><span class="sxs-lookup"><span data-stu-id="96627-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96627-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96627-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96627-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96627-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96627-149">Java</span><span class="sxs-lookup"><span data-stu-id="96627-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96627-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="96627-150">Response</span></span>

<span data-ttu-id="96627-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="96627-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "4b712dc5-2dc5-4b71-c52d-714bc52d714b",
  "relatedContacts": [
      {
          "displayName": "Father Time",
          "emailAddress": "father@time.com",
          "mobilePhone": "4251231234",
          "relationship": "guardian",
          "accessConsent": true
      },
      {
          "displayName": "Mother Nature",
          "emailAddress": "mother@nature.co.uk",
          "mobilePhone": "3251231234",
          "relationship": "parent",
          "accessConsent": true
      }
  ]
}
```
